# 🤖 Minecraft Autonomous Agent

An autonomous agent that plays Minecraft on its own. It starts as a complete beginner, like a brand-new player, and works toward beating the game, making its own decisions along the way instead of following a fixed script.

![Status](https://img.shields.io/badge/status-in%20development-orange)
![Node.js](https://img.shields.io/badge/Node.js-18%2B-green)
![Mineflayer](https://img.shields.io/badge/built%20with-Mineflayer-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

> ⚠️ **Work in progress.** The project is under active development. The source code will be open-sourced once the core agent is stable.

---

## 📖 About

Most Minecraft bots run pre-written scripts: "go here, mine this, craft that." This project aims for something different: an agent that **observes the world, sets its own goals, decides what to do next, and adapts when things go wrong.**

The long-term goal is a bot that can go from an empty inventory to defeating the Ender Dragon with no human help.

## ✨ Goals

- **Autonomous decision-making:** the agent chooses what to do based on what it sees, not a fixed sequence.
- **Goal planning:** it breaks big objectives (like "get diamonds") into smaller steps (wood → tools → stone → iron → diamonds).
- **Adaptation:** it recovers from problems such as dying, running out of food, getting lost or being attacked.
- **Memory:** it remembers important places (base, resources, danger spots) and what it has already tried.
- **Full-game progression:** it plays through the whole game, from the first tree to the Ender Dragon.

## 🧱 Tech Stack

| Tool | Purpose |
|------|---------|
| [Node.js](https://nodejs.org/) | Runtime |
| [Mineflayer](https://github.com/PrismarineJS/mineflayer) | Bot control and game interaction |
| [mineflayer-pathfinder](https://github.com/PrismarineJS/mineflayer-pathfinder) | Navigation and movement |
| [minecraft-data](https://github.com/PrismarineJS/minecraft-data) | Blocks, items and recipe data |
| [prismarine-viewer](https://github.com/PrismarineJS/prismarine-viewer) | Live view of the bot for debugging |

## 🗺️ Roadmap

- [x] Connect the bot to a Minecraft server
- [ ] Reliable movement and pathfinding
- [ ] Resource gathering (wood, stone, food)
- [ ] Crafting and tool progression
- [ ] Survival behavior (eating, sleeping, fighting, fleeing)
- [ ] Goal planner and decision loop
- [ ] Long-term memory
- [ ] Nether progression
- [ ] The End and the Ender Dragon
- [ ] Open-source release

*Update this list as you make progress.*

## 🚀 Getting Started

> Setup instructions will be added when the code is released. The steps below show the expected setup.

### Requirements

- Node.js 18 or newer
- A Minecraft Java Edition server (or a local world opened to LAN)

### Installation

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO
npm install
```

### Configuration

Create a `.env` file in the project root:

```env
MC_HOST=localhost
MC_PORT=25565
MC_USERNAME=AgentBot
```

### Run

```bash
npm start
```

Open `http://localhost:3007` in your browser to watch the bot through prismarine-viewer.

## 🤝 Contributing

Contributions will open up after the first public release. Ideas and feedback are welcome now. Open an issue to start a discussion.

## 📄 License

Planned release under the [MIT License](LICENSE).

## 🙏 Acknowledgements

Built on the excellent work of the [PrismarineJS](https://github.com/PrismarineJS) community.
