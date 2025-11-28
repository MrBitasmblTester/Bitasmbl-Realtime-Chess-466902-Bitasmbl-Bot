# Bitasmbl-Realtime-Chess-466902-Bitasmbl-Bot

## Description
Design and implement a real-time, web-based chess application where two authenticated players can join a lobby, start a match, and play live against each other. The system must handle valid chess moves, turn-based state management, and reliable client–server synchronization using a React front end and a Node.js backend.

## Tech Stack
- React
- Node.js
- Socket.IO

## Requirements
- Validate chess moves on the server so illegal moves are rejected and the board state remains authoritative.
- Support reconnection so a player can refresh the page and rejoin the same game without losing state.
- Implement basic time control (e.g., 10 minutes per player) and detect timeouts on the server.

## Installation
bash
git clone https://github.com/MrBitasmblTester/Bitasmbl-Realtime-Chess-466902-Bitasmbl-Bot.git
cd Bitasmbl-Realtime-Chess-466902-Bitasmbl-Bot
npm install
cd client
npm install


## Usage
bash
# In project root
npm run server
# In client directory
npm start


## Implementation Steps
1. Set up Node.js server with Socket.IO to manage lobbies, matches, and real-time events.
2. Implement server-side chess board representation, move validation, and turn-based state updates.
3. Add basic time control per player and server-side timeout detection.
4. Implement reconnection logic binding players to existing games by their authenticated identity.
5. Build React UI for lobby, game board, timers, and live move updates via Socket.IO.
6. Ensure server remains the single source of truth and clients render server-confirmed state.

## API Endpoints
- WebSocket events for lobby join, game start, move submission, state sync, and reconnection.