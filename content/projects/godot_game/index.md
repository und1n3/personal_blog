---
title: "Designing a booknook"
date: 2024-06-25
draft: false
project_tags: ["booknook","3d","3dprinting","blender"]
status: "withered"
weight: 2
summary: "Example of markdown syntax you can use to edit your content"
links:
    external_link:
        text: "Some external link"
        icon: "fas fa-external-link-alt"
        href: "#"
        weight: 1
    another_link:
        text: "Another github link"
        icon: "fab alt brands fa-github"
        href: "#"
        weight: 2
---
# ⚔️ 2-Day Game Jam Schedule: "Cable Crawler"

## 🎮 Game Summary
- **Genre:** Top-down stealth-action
- **Theme:** Expedition (but you're the villain)
- **Goal:** Steal relics from a peaceful alien world accessed through your computer cable
- **Twist:** You’re the invader
- **Audio:** All sounds are made using acapella (mouth/voice)

---

## 🗓️ DAY 1 — Core Systems & Foundation

### 🕗 Hour 1: Project Setup
- [x] Create new Godot project
- [ ] Set up basic scenes:
  - `Main.tscn`
  - `Player.tscn`
  - `Enemy.tscn`
  - `Level01.tscn`
- [ ] Add camera that follows player

### 🕘 Hour 2: Player Movement + Stealth
- [ ] 2D movement + collision
- [ ] Add light radius (for glow power-up)
- [ ] Boolean flag `is_hidden`
- [ ] Toggle visibility logic

### 🕙 Hour 3: Enemy AI + Vision Cone
- [ ] Enemy patrols between points
- [ ] Area2D + raycasts or polygon cone for vision
- [ ] Detect player if not hidden

### 🕚 Hour 4: Power-Up System (Part 1)
- [ ] Create `PowerUp.gd` base scene
- [ ] Light Core: turns on glow + increases detection
- [ ] Simple pickup logic + timer/cooldown

### 🕛 Hour 5: Map Building
- [ ] Use TileMap or grid-based layout
- [ ] Build 1–2 rooms with walls, floor, objects
- [ ] Place 1 relic to collect

### 🕐 Hour 6: UI + Relic Tracking
- [ ] Basic HUD for relics collected (3 total)
- [ ] Icon toggle or number display
- [ ] (Optional) power-up icon indicator

### 🕑 Hour 7: Sound Framework
- [ ] Set up AudioStreamPlayer nodes
- [ ] Import sample acapella sounds:
  - Walking
  - Power-up use
  - Alert

### 🕒 Hour 8: Playtest + Polish
- [ ] Refine player movement and stealth feel
- [ ] Adjust enemy vision/debug print
- [ ] Clean up code and visuals

---

## 🗓️ DAY 2 — Content, Boss, Polish

### 🕗 Hour 1: Add Dark Fruit Power-Up
- [ ] Temporary invisibility (5s)
- [ ] Visual cue (dim player or screen)
- [ ] Enemies ignore player when active

### 🕘 Hour 2: Add Sonic Blaster
- [ ] Area2D cone or Raycast weapon
- [ ] Knocks out enemies temporarily
- [ ] Adds noise risk (optional alert)

### 🕙 Hour 3: Final Room + Boss Zone
- [ ] Add third room (final relic)
- [ ] Tougher enemy or gate puzzle
- [ ] End trigger: all relics collected

### 🕚 Hour 4: Finalize Level Design
- [ ] Place 3 relics across map
- [ ] Add patrol routes + cameras or light hazards
- [ ] Optional: terminal logs / carvings

### 🕛 Hour 5: Sound Pass (Acapella Only)
- [ ] Record:
  - Footsteps
  - Power-ups
  - Alerts
  - Blaster sound
  - Relic pickup
- [ ] Add variation (pitch, random delay)

### 🕐 Hour 6: Ending Sequence
- [ ] Final screen or fade out
- [ ] “You are the invader…” message
- [ ] Optional: aliens stop attacking

### 🕑 Hour 7: Bug Fixing + Polish
- [ ] Particles, screen shake, UI polish
- [ ] Code cleanup + organize assets
- [ ] Fix enemy glitches or AI hiccups

### 🕒 Hour 8: Playtest + Export
- [ ] Full run test from start to end
- [ ] Export to Web or EXE
- [ ] Create itch.io page (optional)

---

## 🛠️ Target Specs

| Setting       | Value         |
|---------------|---------------|
| Resolution    | 1280x720 px   |
| Tile Size     | 32x32 px      |
| Player Sprite | 32x32 or 24x32|
| Tileset Canvas| 256x256+ px   |
| Filtering     | Off (pixel-perfect) |
| Stretch Mode  | Viewport / Keep |
