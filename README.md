# ♟️ Multiplayer Chess Game

A real-time multiplayer chess game built with Node.js, Socket.IO, and chess.js. Play chess with friends in real-time with automatic role assignment and spectator support.

<div align="center">
  <img src="https://github.com/user-attachments/assets/b4c86729-d5f1-4290-a074-35de7517596a" 
       alt="Chess Game Demo" 
       width="400"
       style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
</div>

## ✨ Features

- **Real-time multiplayer** - Play with friends instantly
- **Drag & drop interface** - Intuitive piece movement
- **Automatic role assignment** - First player white, second black, rest spectators
- **Turn validation** - Only current player can move
- **Board flipping** - Black player's view automatically rotated
- **Server-side validation** - All moves checked for legality
- **Spectator mode** - Unlimited viewers can watch games

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Node.js + Express | Backend server |
| Socket.IO | Real-time communication |
| chess.js | Chess logic & validation |
| HTML5/CSS3 | Frontend structure |
| Tailwind CSS | Styling framework |
| EJS | Templating |

## 📁 Project Structure

| File/Folder | Description |
|-------------|-------------|
| app.js | Main server file (Node.js/Express) |
| package.json | Project dependencies and scripts |
| style.css | Custom styling for chessboard |
| chessgame.js | Frontend game logic |
| backendSetup.yaml | Backend architecture documentation |
| frontendSetup.yaml | Frontend architecture documentation |
| views/index.ejs | Game template (EJS) |

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/arhamofficial06/Chess-Game.git
   cd Chess-Game

2. **Install dependencies**
   ```bash
   npm install
3. **Start the server**
   ```bash
   npm run nodemon
   # or
   node app.js
4. **Open in browser**
   ```bash
   http://localhost:3000
🎮 How to Play
1. Open the game in two different browser windows/devices

2. First player gets white pieces automatically

3. Second player gets black pieces automatically

4. Others become spectators

5. Drag & drop pieces to make moves

6. Wait for your turn - game enforces turn order

7. Spectators watch in real-time without interaction

## 📡 Socket Events

| Event | Direction | Description |
|-------|-----------|-------------|
| `playerRole` | Server → Client | Assigns player role (w/b) |
| `spectatorRole` | Server → Client | Assigns spectator role |
| `boardState` | Server → Client | Sends FEN board state |
| `move` | Both | Sends/receives moves |
| `invalidMove` | Server → Client | Invalid move notification |

## 🎨 Customization

### Styling
- Edit `style.css` for board colors and piece styling
- Modify Tailwind classes in `index.ejs`

### Piece Graphics
Current implementation uses Unicode characters. To use custom images:

```javascript
// In chessgame.js - modify getPieceUnicode function
const getPieceUnicode = (piece) => {
  // Replace with image tags or custom icons
};
```
## 🤝 Contributing

Contributions welcome! Feel free to:

- 🐛 **Report bugs** - Open an issue with detailed description
- 💡 **Suggest features** - Share your ideas for improvements
- 🔧 **Submit pull requests** - Fork the repo and create a PR

## 📝 License

ISC License - use freely for personal and commercial projects.

## 📞 Contact

- **GitHub**: [@arhamofficial06](https://github.com/arhamofficial06)
- **Project Link**: [https://github.com/arhamofficial06/Chess-Game](https://github.com/arhamofficial06/Chess-Game)

## 🙏 Acknowledgments

- [chess.js](https://github.com/jhlywa/chess.js) for chess logic
- [Socket.IO](https://socket.io/) for real-time communication
- [Tailwind CSS](https://tailwindcss.com/) for styling

---

⭐ **Star this repo if you found it helpful!**  
**Happy Playing! ♟️**