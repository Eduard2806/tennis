# Tennis Match Scheduler Design

## Architecture
- Next.js frontend application
- Single page with form input and schedule display
- Client-side schedule generation

## Algorithm
With 4 players (A, B, C, D), each playing 2 matches:
- Total matches needed: 4 players × 2 matches ÷ 2 = 4 matches
- Possible pairings: AB, AC, AD, BC, BD, CD (6 total)
- Select 4 pairings ensuring each player appears exactly twice

## Solution
Use round-robin approach:
1. Match 1: A vs B
2. Match 2: C vs D  
3. Match 3: A vs C
4. Match 4: B vs D

This ensures each player plays exactly 2 matches.

## Components
- PlayerInput: Form to enter 4 player names
- ScheduleDisplay: Shows generated match schedule
- Main page: Combines both components
