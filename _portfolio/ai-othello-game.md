---
title: "AI Othello Game: Design and Implementation in C#"
excerpt: "My undergraduate thesis project, an Othello (Reversi) game developed in C#. It features a custom AI with a phased composite strategy, full game functionality including replay and file I/O, and was built on the .NET Framework."
layout: custom
header:
  image: /images/portfolio-ai-othello.jpg
  teaser: /images/portfolio-ai-othello.jpg
order: 6
collection: portfolio
author_profile: true
---

# AI Othello Game: Design and Implementation in C#

## Project Overview

This project is my undergraduate thesis, titled "Design and Implementation of an Othello Game based on C#". Supervised by Prof. Wei Xu, this project involved building a complete, feature-rich Othello (Reversi) game application from the ground up. The core of the project was to develop an intelligent game-playing AI agent by designing and implementing a composite heuristic strategy, rather than relying on a single algorithm. The entire system was developed using C# on the .NET platform.

![Game Interface](/images/portfolio/othello-gameplay-midgame.png)
*AI Othello game in action - demonstrating the intuitive interface and strategic gameplay*

## 🎯 Project Objectives & Key Features

Based on the analysis of player needs, this game software was developed to include a comprehensive set of features providing a high-quality user experience.

* **Game Modes**:
    * **Two-Player Mode**: For local head-to-head gameplay.
    * **Human-Computer Mode**: Play against an AI with multiple difficulty levels (from beginner to advanced).
    * **Spectator Mode**: Watch two AIs of different difficulties play against each other.
* **Core Gameplay Functionality**:
    * **Move Undo/Redo**: Allows players to take back moves and restore them.
    * **Full Game Replay**: A "Full Game Replay" feature to review a completed game from the first move.
    * **Custom Time Limits**: Players can set a custom total time limit for games.
* **Data Persistence**:
    * **Save/Load Games**: Manually save the current game state to a `.csv` file.
    * **Import Game Records**: Load game records from external `.csv` files or by pasting text.
    * **Automatic History**: Every game is automatically saved to a history `.txt` file and can be reloaded by its number.

![Game Start Interface](/images/portfolio/othello-start-interface.png)
*Clean game start interface showing the initial board setup and control options*

## 🔧 Technical Approach

### AI Strategy: A Phased, Composite Approach

Through testing, it was found that single strategies (like pure greedy or positional) had significant weaknesses. Therefore, the AI does not use a simple Minimax algorithm but a **phased composite strategy** that adapts based on the stage of the game, aiming to replicate the thinking of a human intermediate player.

1.  **Opening Game (First few moves)**: The AI employs a **Mobility Strategy**. The goal is to maximize its own move options while minimizing the opponent's, forcing the human player into making non-ideal moves early on.

2.  **Mid-Game**: The AI switches to a combination of **Positional Strategy** and **Mobility Strategy**. It prioritizes securing strategic positions while continuing to restrict the opponent's movement.

3.  **Endgame**: In the final phase of the game, the AI adopts a pure **Greedy Strategy**, aiming to maximize its final piece count to secure the win.

![AI Decision Making](/images/portfolio/othello-ai-thinking.png)
*AI strategy in action - showing move hints and strategic positioning*

### System Architecture & Key Technologies
The system was designed and built using the following technologies:
* **Programming Language**: **C#**
* **Framework**: **.NET Framework**
* **Development Environment**: **Visual Studio 2019**
* **User Interface**: Windows Forms, with a custom-drawn GDI+ game board and UI elements.
* **Data Persistence**: The **`System.IO`** namespace was used extensively to read from and write to `.txt` and `.csv` files for all save/load and history functions.

## 🎨 User Interface & Design

### Visual Themes
The game features multiple visual themes to enhance user experience:

![Green Theme Interface](/images/portfolio/othello-green-theme.png)
*Traditional green board theme providing a classic Othello experience*

![Classic Theme Interface](/images/portfolio/othello-classic-theme.png)
*Modern black and white theme for a sleek, contemporary look*

### Game Flow and User Experience
The interface is designed for intuitive gameplay with clear visual feedback:

- **Real-time Score Display**: Live updates of piece counts
- **Move History Tracking**: Complete game record with step-by-step replay
- **Visual Move Indicators**: Clear highlighting of legal moves
- **Game State Management**: Easy save/load functionality

![Move History Feature](/images/portfolio/othello-move-history.png)
*Comprehensive move history and game replay functionality*

## 📊 Project Outcomes & Conclusion

The project was successfully completed, meeting all the initial design requirements.
* **Functionality**: All planned features, including the various game modes, undo/redo, replay, and comprehensive import/export functions, were fully implemented and tested over 15 days with 676 test cases.
* **AI Performance**: The final AI, using the phased composite strategy, achieved a level evaluated to be **comparable to a human intermediate player**.
* **Usability**: The software provides a user-friendly interface and a stable, high-quality gaming experience for Othello enthusiasts.

![Game Victory Screen](/images/portfolio/othello-endgame-victory.png)
*Game completion showing final scores and victory announcement*

## 🔮 Future Enhancements

As noted in the thesis, while the project was successful, there are areas for future improvement.
* **Deeper AI Optimization**: The current AI algorithm is effective but still considered at a relatively basic stage. Future work would involve researching and implementing more advanced search techniques and self-learning models to further enhance the AI's strength.
* **Feature Completion**: Add the option for the player to choose "White" (moving second) in all game modes, a feature which was planned but not fully implemented due to time constraints.

## 📈 Technical Skills Demonstrated

* **Software Engineering**: Full lifecycle development from requirements analysis, system design, implementation, to testing.
* **Object-Oriented Programming (C#)**: Application of OOP principles to build a complex, interactive application.
* **Algorithm Design**: Design and implementation of a custom, rule-based AI strategy beyond simple algorithms.
* **UI/UX Design**: Creation of an intuitive and functional graphical user interface for a game application.
* **File I/O**: Practical use of file streams for data serialization and persistence.

---

*This project was a comprehensive exercise in software development and an exploration into the fascinating field of game AI. It provided a solid foundation in building applications from concept to completion and tackling the logic of strategic decision-making in code.*