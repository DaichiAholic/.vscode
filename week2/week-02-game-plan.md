```mermaid
mindmap
 root((Pac-Man))
  Theme
   เขาวงกต
   อาเขตยุค 80
  Mechanics
   เดินในเขาวงกต
   กิน Pellet
   Power Pellet
  Content
   ผีศัตรู 4 ตัว
   ผลไม้โบนัส
  Audience
   ผู้เล่น Casual
  sound
   เพลงประกอบ
   environment sound
```

```mermaid
quadrantChart
 title Pac-Man — Feature Prioritization
  x-axis Low Effort --> High Effort
  y-axis Low Impact --> High Impact
 quadrant-1 Quick Wins
 quadrant-2 Major
 quadrant-3 Nice to Have
 quadrant-4 Reconsider
 Maze Movement: [0.3, 0.95]
 Ghost AI: [0.7, 0.9]
 Online Leaderboard: [0.7, 0.3]
 Lives / Game Over: [0.1, 0.9]
 SFX + jingle: [0.1,0.6]
 Cutscene: [0.4,0.4]
 bonus fruit: [0.7,0.4]
```

1. MVP -- Live / Game Over, SFX + jingle, Ghost AI, Maze Movement : สำคัญเพราะทำให้เกมสนุกและตื่นเต้น
2. ตัดออก -- Online Leaderboard, cutscrene, bonus fruit: ตัดออกเพราะไม่ได้สำคัญขนาดนั้นแต่ถ้ามีเวลาก็ทำได้

```mermaid
gantt
title Pac-Man — Production Timeline (6 สัปดาห์)
dateFormat YYYY-MM-DD
section Pre-Production
Concept & GDD :done, c1, 2026-07-06, 5d 

section Production
SFX + jingle :active, p1, after c1, 3d
Maze Movement :active, p1, after c1, 5d
Ghost AI : p2, after p1, 7d
Pellet & Score : p3, after p2, 7d

section Alpha
Test : milestone ,p4, after p3, 2d

section Post
QA & Bug Fix : active p4, after p4, 5d
Release Build :milestone, m1, after q1, 0d

```
