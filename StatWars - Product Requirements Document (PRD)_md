#  StatWars - Product Requirements Document (PRD)

## Overview

StatWars is an **NBA-focused social competitive platform** where users play mini-games, challenge friends, and test their basketball knowledge.

The platform combines:
-  Interactive gameplay  
-  Knowledge-based challenges  
-  Social competition  

---

##  Product Vision

To build a **competitive social platform** where NBA fans can:
- Compete with others  
- Improve their knowledge  
- Engage through multiple mini-games  

---

##  Success Metrics

- **North Star Metric:** Daily number of games played  
- **Engagement Metric:** Average games per user  
- **Virality Metric:** Number of game invites per user  

---

##  Tech Stack

- **Frontend:** React (Next.js)
- **Backend:** Node.js (Express / NestJS)
- **Realtime:** WebSockets (Socket.io)
- **Database:** Supabase (PostgreSQL)
- **Auth:** Supabase Auth / JWT
- **Hosting:** Vercel + Render / Railway

---

##  Core Game Modes

### 1. Card Battle (Primary Game)
- Each player receives 5 NBA player cards  
- A random stat appears each round (points, rebounds, assists)  
- Players select a card  
- Highest stat wins the round  

---

### 2. Ranking Game
- Users are given 5 players  
- They must rank them based on a stat  
- Points awarded based on accuracy  

---

### 3. Trivia / Guess Game
- Example: “Who has the most rebounds in NBA history?”  
- User selects or inputs an answer  

---

### 4. Weekly Fantasy Quiz (Planned)
- Weekly competition  
- Leaderboard-based ranking  
- Monetization potential  

---

##  Database Schema (Simplified)

### users
- id (UUID)
- username (string)
- created_at (timestamp)

### games
- id (UUID)
- type (string)
- status (waiting / active / finished)
- created_at (timestamp)

### game_players
- id (UUID)
- game_id (FK)
- user_id (FK)
- score (integer)

### nba_players
- id (UUID)
- name (string)
- points (float)
- rebounds (float)
- assists (float)

---

##  API Endpoints (Examples)

- POST `/auth/register`
- POST `/auth/login`

- POST `/game/create`
- POST `/game/join`
- GET `/game/:id`

- POST `/game/play-turn`
- GET `/leaderboard`

---

##  Screens & User Flow

### Home Screen
- Game selection  
- Play buttons  

### Game Lobby
- Player list  
- Start game button  

### Game Screen
- Player cards  
- Current stat display  
- Selection interface  

### Result Screen
- Winner display  
- Score summary  

### Leaderboard
- Global rankings  

---

##  User Stories

### US 1 – Create & Join Game
- Users can create a game  
- Users can invite friends  

---

### US 2 – Play Game Turns
- Users select a card each round  
- Results are shown instantly  

---

### US 3 – Ranking Gameplay
- Users can reorder players  
- Correct ranking is displayed  

---

##  MVP Scope

###  Included in MVP

- User authentication  
- Card Battle game mode  
- Basic multiplayer (2 players)  
- Leaderboard  
- Simple UI  

---

###  Excluded from MVP

- Real money rewards  
- Weekly fantasy system  
- Power-ups / abilities  
- Advanced AI  
- Full social system  

---

##  MVP Strategy

Goal:

> Validate if users enjoy and replay the game

### Key Metrics:
- Daily Active Users (DAU)  
- Replay rate  
- Average session duration  

---

## Roadmap

- Add Ranking Game  
- Add Trivia Game  
- Improve multiplayer  
- Add weekly tournaments  
- Add reward system  
- Build mobile app  

---

## Out of Scope (Phase 1)

- Real money rewards  
- Advanced matchmaking  
- AI-based personalization  
- Native mobile apps  

---

## Notes

StatWars is designed as a scalable platform where new game modes can be added over time.

This document defines the MVP scope and technical foundation.