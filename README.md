# Life RPG - Complete Game Guide

## 📖 Table of Contents
1. [Game Overview](#game-overview)
2. [Getting Started](#getting-started)
3. [Character System](#character-system)
4. [Visual Character Upgrades](#visual-character-upgrades)
5. [Experience & Leveling](#experience--leveling)
6. [Daily Quests](#daily-quests)
7. [Anytime Tasks](#anytime-tasks)
8. [Cooldown System](#cooldown-system)
9. [Character Upgrades](#character-upgrades)
10. [Boss Battles](#boss-battles)
11. [Statistics Tracking](#statistics-tracking)
12. [Tips & Strategies](#tips--strategies)
13. [Technical Details](#technical-details)

---

## Game Overview

**Life RPG** is a gamified self-improvement web application that transforms your daily activities into an engaging RPG experience. By completing real-life tasks like exercising, drinking water, and learning new things, you earn experience points (XP) and skill points to upgrade your character.

### Core Concept
- Turn healthy habits into rewarding gameplay
- Visual character progression that reflects your improvements
- No account required - all progress saved locally in your browser
- Designed for mobile and desktop use

### Game Loop
1. **Complete Tasks** → Earn XP and Skill Points
2. **Level Up** → Unlock new features and tasks
3. **Upgrade Character** → See visual transformations
4. **Fight Bosses** → Earn massive rewards
5. **Build Streaks** → Maintain consistency

---

## Getting Started

### First Launch
When you first open the game:
1. You start at **Level 1** with 0 XP
2. Your character appears as a basic SVG avatar
3. All Level 1 tasks are available
4. No skill points yet (earn them by completing tasks)

### Interface Overview

**Character Card (Top)** - Blue gradient card displaying:
- Character avatar (animated SVG)
- Character name (editable)
- Current level badge
- XP progress bar showing progress to next level
- Four stat boxes:
  - Total XP (cumulative)
  - Skill Points (available to spend)
  - Quests Done (total count)
  - Day Streak (consecutive days)

**Character Upgrades Section** - Where you spend skill points on 4 attributes

**Daily Quests Section** - Tasks that reset at midnight

**Anytime Tasks Section** - Repeatable tasks with cooldowns

**Explore the World Section** - Boss battles (unlocks at Level 2)

---

## Character System

### Your Avatar

Your character is represented by a **fully animated SVG illustration** that visually changes as you upgrade your stats. The character design includes:

**Base Character (Level 0 Stats):**
- Round head with simple facial features
- Normal-sized arms and torso
- Standard blue shirt/torso
- Black pants/legs
- Neutral skin tone
- Glowing aura around the avatar (always present)

**Character Evolution:**
As you upgrade different stats, your character's appearance transforms in real-time with smooth animations.

---

## Visual Character Upgrades

### 💪 Physical Strength Upgrades

**What Changes:**
- **Arms grow larger and more muscular**
- **Chest (pectoral muscles) expand**
- **Abdominal muscles become more defined**
- **Overall body size increases**
- **Torso becomes broader**

**Visual Progression:**

**Level 0-2 Strength:**
- Skinny arms (15px width)
- Flat chest
- No visible muscle definition
- Basic body proportions

**Level 3-5 Strength:**
- Arms grow to 18px width
- Small bicep bumps visible
- Chest muscles start to show (pecs appear)
- Abs become slightly defined
- Body scales up by 15%

**Level 6-9 Strength:**
- Muscular arms (20px width)
- Prominent biceps with clear definition
- Well-defined chest muscles (expanded pecs)
- Six-pack abs clearly visible
- Body scales up by 30%

**Level 10+ Strength:**
- **HUGE muscular arms** (25px+ width)
- **Massive biceps** bulging visibly
- **Very large chest muscles** (pecs significantly expanded)
- **Ultra-defined eight-pack abs**
- **Body scaled up by 50%+** - true bodybuilder physique!
- Biceps are 50% larger in diameter
- Chest muscles extend outward prominently

**Technical Details:**
- Each strength level increases arm scale by 5%
- Pectoral muscles (ellipses) grow in both width (rx) and height (ry)
- Muscle stroke width increases for definition
- Smooth 0.5-second transitions between levels
- Transform origin is centered for natural scaling

---

### ❤️ Endurance Upgrades

**What Changes:**
- **Heart becomes visible in chest**
- **Heart beats faster and more prominently**
- **Heart color intensifies (brighter red)**
- **Heart grows slightly larger**
- **Beating animation speed increases**

**Visual Progression:**

**Level 0 Endurance:**
- No heart visible
- No cardiovascular indicator

**Level 1-3 Endurance:**
- Small red heart appears in chest (50% opacity)
- Slow beating animation (1.5 seconds per beat)
- Subtle presence
- Light red color (#ff4444)

**Level 4-6 Endurance:**
- Heart becomes more prominent (70% opacity)
- Medium beat speed (1.0 seconds per beat)
- Brighter red color
- Slightly larger heart
- More noticeable pulsing effect

**Level 7-9 Endurance:**
- Very prominent heart (85% opacity)
- Fast beating (0.7 seconds per beat)
- Vibrant red color
- Clearly visible and energetic

**Level 10+ Endurance:**
- **Maximum prominence** (100% opacity)
- **Rapid heartbeat** (0.5 seconds per beat)
- **Intense bright red** color
- **Dynamic pulsing** animation
- Shows peak cardiovascular fitness!

**Technical Details:**
- Heart uses path SVG element for realistic shape
- Animation duration decreases with higher endurance
- Opacity increases 5% per level
- Heartbeat uses scale transform (1.0 → 1.1 → 1.0)
- Transform origin centered on heart
- CSS animation: `heartbeat` keyframes

---

### 🧠 Intelligence Upgrades

**What Changes:**
- **Brain icon appears inside head**
- **Golden glow emanates from brain**
- **Pulsing light effect around head**
- **Glow brightness increases**
- **Aura expands outward**

**Visual Progression:**

**Level 0 Intelligence:**
- No brain indicator visible
- Standard head appearance
- No special effects

**Level 1-3 Intelligence:**
- Small golden brain icon appears (10% opacity)
- Very faint glow
- Minimal light emission
- Brain outline barely visible

**Level 4-6 Intelligence:**
- Brain icon becomes clearer (40% opacity)
- Moderate golden glow
- Soft light halo around head
- Gentle pulsing effect (2-second cycle)
- Golden yellow color (#ffd700)

**Level 7-9 Intelligence:**
- Prominent brain visible (70% opacity)
- Strong golden glow
- Noticeable light aura
- Faster pulsing (1.5-second cycle)
- Bright illumination effect

**Level 10+ Intelligence:**
- **Brilliant glowing brain** (100% opacity)
- **Intense golden radiance**
- **Large light aura** surrounding entire head
- **Rapid pulsing** (1-second cycle)
- **Dramatic drop-shadow** effect (0-15px glow)
- Represents genius-level intellect!

**Technical Details:**
- Brain drawn with path SVG for anatomical shape
- Uses CSS filter: drop-shadow for glow effect
- Opacity increases 10% per level
- Pulsing animation: `brainPulse` keyframes
- Glow expands from 5px to 15px radius
- Golden color transitions smoothly

---

### 🏅 Discipline Upgrades

**What Changes:**
- **Golden ring (aura) surrounds character**
- **Ring continuously rotates**
- **Ring gets thicker**
- **Ring becomes brighter/more opaque**
- **Rotation speed stays constant**

**Visual Progression:**

**Level 0 Discipline:**
- No aura visible
- No special effects around character
- Standard appearance

**Level 1-3 Discipline:**
- Thin golden ring appears (2px thick)
- Faint visibility (20% opacity)
- Slow rotation (4-second full rotation)
- Circle positioned around outer edge of avatar

**Level 4-6 Discipline:**
- Medium thickness ring (4px thick)
- Moderate visibility (40% opacity)
- Steady rotation
- More noticeable presence
- Golden color (#ffd700)

**Level 7-9 Discipline:**
- Thick golden ring (6px thick)
- Strong visibility (60% opacity)
- Clear golden aura
- Prominent rotating effect
- Shows strong willpower

**Level 10+ Discipline:**
- **Very thick ring** (8px+ thick)
- **Maximum visibility** (80% opacity)
- **Brilliant golden aura**
- **Continuous smooth rotation**
- **Represents mastery and focus**
- Ring appears as powerful force field!

**Technical Details:**
- Circle SVG element (radius 90px)
- Stroke-only (no fill) for ring effect
- CSS transform: rotate() animation
- Stroke-width increases with level (+1px per level)
- Opacity increases 8% per level
- Animation: `rotateAura` keyframes (4s linear infinite)
- Transform origin: center (100px, 100px)

---

### 🎨 Combined Visual Effects

**What happens when you upgrade multiple stats:**

**All Stats at Level 5:**
- Medium muscular build
- Beating heart visible
- Glowing brain with light aura
- Rotating golden ring
- Balanced, well-rounded appearance
- All effects work together harmoniously

**All Stats at Level 10:**
- **Massive muscular physique**
- **Rapid heartbeat** pulsing visibly
- **Brilliant glowing brain** radiating golden light
- **Thick rotating golden aura** surrounding everything
- **Maximum visual impact**
- Character looks like a superhero/demigod!

**Mixed Stats Example (Fighter Build):**
- Strength 15, Endurance 10, Intelligence 2, Discipline 5
- **Huge muscles** dominating the appearance
- **Strong heartbeat** showing stamina
- Minimal brain glow
- Moderate golden ring
- Looks like a powerful athlete

**Mixed Stats Example (Scholar Build):**
- Strength 3, Endurance 5, Intelligence 15, Discipline 12
- Normal body size with slight muscle tone
- Moderate heartbeat
- **Brilliant glowing brain** as main feature
- **Very thick golden aura** showing focus
- Looks like an enlightened sage

---

## Experience & Leveling

### Experience Points (XP)

**How to Earn XP:**
- Complete daily quests (15-30 XP each)
- Complete anytime tasks (10-50 XP each)
- Defeat bosses (50-100 XP each)

**XP Requirements:**
- Level 1 → 2: **100 XP**
- Level 2 → 3: **200 XP**
- Level 3 → 4: **300 XP**
- Level N → N+1: **N × 100 XP**

**Formula:** XP needed for next level = Current Level × 100

**Example Progression:**
```
Level 1: 0/100 XP needed
Level 2: 0/200 XP needed  (100 XP earned total)
Level 3: 0/300 XP needed  (300 XP earned total)
Level 5: 0/500 XP needed  (1000 XP earned total)
Level 10: 0/1000 XP needed (4500 XP earned total)
```

### Level Up Rewards

**Every time you level up:**
- 🎁 **+3 Skill Points** (to spend on upgrades)
- 🎊 **Unlock notification** with celebration message
- 🔓 **May unlock new content:**
  - Level 2: Unlocks "Explore the World" (boss battles)
  - Level 2: Unlocks additional daily quests
  - Level 3: Unlocks more anytime tasks
  - Level 4: Unlocks harder bosses

**Visual Changes:**
- XP bar resets to 0 and shows new requirement
- Level badge updates in character card
- Avatar gets a brief glow effect
- Success notification appears at top

**XP Progress Bar:**
- Located below character name
- Yellow/gold color with animated stripes
- Shows current XP / required XP
- Example: "150 / 200" means 150 out of 200 XP earned
- Fills from left to right
- Smooth transition when earning XP

---

## Daily Quests

### Overview
Daily quests are healthy habits you should complete **once per day**. They reset at midnight every day.

### Quest List

| Quest | XP | Skill Points | Min Level | Description |
|-------|----|--------------|-----------| ------------|
| 🏃 Exercise for 15 minutes | 20 | 1 | 1 | Physical activity of your choice |
| 💧 Drink 8 glasses of water | 15 | 1 | 1 | Stay hydrated throughout the day |
| 📚 Learn something new for 30 min | 25 | 2 | 1 | Read, study, or take a course |
| 😴 Sleep 8 hours | 20 | 1 | 1 | Get full night's rest |
| 🧘 Meditate for 10 minutes | 30 | 2 | 2 | Practice mindfulness |
| 🍎 Eat a healthy meal | 15 | 1 | 2 | Nutritious whole foods |
| 📖 Read for 30 minutes | 25 | 2 | 3 | Books or educational content |
| 👥 Connect with a friend/family | 20 | 1 | 3 | Social interaction |

### Quest Mechanics

**Status Indicators:**
- ✅ **Green checkmark** = Completed today
- 🔓 **Available** = Ready to complete
- 🔒 **Red lock icon** = Requires higher level

**Completion:**
1. Click "Complete" button next to quest
2. Immediately receive XP and skill points
3. Quest becomes grayed out with checkmark
4. Can't complete again until next day

**Daily Reset:**
- Happens at **midnight (00:00)** in your local time
- All completed quests become available again
- Checkmarks disappear
- Fresh start each day

**Streak System:**
- Completing ANY daily quest counts toward streak
- Consecutive days of completion = streak
- Skip a day = streak resets to 0
- Displayed as "Day Streak" in stats
- Encourages daily engagement

**Visual Design:**
- White cards with left blue border (5px)
- Quest icon at start
- Quest name in bold
- Reward info below (XP and skill points)
- Purple "Complete" button on right
- Completed quests have 60% opacity
- Locked quests have 50% opacity with red border

---

## Anytime Tasks

### Overview
Anytime tasks are activities you can complete **multiple times** throughout the day. Unlike daily quests, they don't reset - you can do them whenever you want!

### Task List

| Task | XP | Skill Points | Min Level | Cooldown |
|------|----|--------------|-----------| ---------|
| 💪 Do 20 push-ups | 10 | 0 | 1 | 1 hour |
| 🚶 Take a 15-minute walk | 15 | 1 | 1 | 1 hour |
| 🧹 Clean/organize your space | 20 | 1 | 1 | 1 hour |
| 🚿 Take a cold shower | 25 | 1 | 1 | 1 hour |
| 🤝 Help someone in need | 30 | 2 | 1 | 1 hour |
| 📝 Write in journal (5+ minutes) | 20 | 1 | 2 | 1 hour |
| 🍳 Cook a healthy meal from scratch | 35 | 2 | 2 | 1 hour |
| 🎸 Practice a skill for 30 minutes | 30 | 2 | 2 | 1 hour |
| 📵 No phone for 2 hours | 40 | 2 | 3 | 1 hour |
| 🏋️ Complete intense workout (45+ min) | 50 | 3 | 3 | 1 hour |
| 👨‍🏫 Teach someone something new | 35 | 2 | 3 | 1 hour |
| 🎨 Create something artistic | 40 | 2 | 4 | 1 hour |

### Task Mechanics

**Completion Count:**
- Green badge shows how many times completed
- Example: **"3x"** means completed 3 times
- Counter increases with each completion
- Tracked forever (doesn't reset)

**Status Indicators:**
- 🟢 **Green "Complete" button** = Ready to do
- ⏰ **Red timer badge** = On cooldown (shows time remaining)
- 🔒 **Lock icon** = Requires higher level
- ⏸️ **Gray "Wait" button** = Global cooldown active

**Rewards:**
- Instant XP gain
- Instant skill points (if any)
- Adds to total quest completion count
- Updates character stats immediately

**Visual Design:**
- Similar to daily quests but with distinct features
- Completion counter badge in green
- Red cooldown timer when active
- Semi-transparent appearance when on cooldown
- Icon at start shows task type
- No checkmark (since can repeat)

---

## Cooldown System

### Two Types of Cooldowns

#### 1. Global Refractory Period (30 Seconds)

**What is it?**
A short "cool down" period after completing ANY anytime task that prevents you from completing OTHER tasks immediately.

**Why it exists:**
- Prevents "trigger happy" clicking
- Encourages intentional task completion
- Prevents gaming the system
- Promotes mindfulness

**What happens:**
1. You complete an anytime task
2. **RED BANNER appears** at top of anytime tasks section
3. Banner says: **"⏳ Refractory Period"**
4. Shows countdown: **"Wait 30s before completing another task"**
5. **White progress bar** shows time remaining visually
6. **ALL anytime task buttons become disabled**
7. Buttons change from "Complete" to gray "Wait"
8. After 30 seconds, banner disappears automatically
9. Other tasks become available again

**Visual Features:**
- Red/pink gradient banner with pulsing animation
- Countdown timer updates every second (30, 29, 28...)
- Progress bar drains from 100% to 0%
- Smooth animation
- All task cards become semi-transparent (50% opacity)

**Technical Details:**
- Duration: 30,000 milliseconds (30 seconds)
- Updates every 100ms for smooth animation
- Banner auto-removes when cooldown expires
- Prevents all task completions during this time

#### 2. Individual Task Cooldown (1 Hour)

**What is it?**
Each specific task has its own 1-hour cooldown before you can do THAT SAME task again.

**Why it exists:**
- Prevents spamming the same easy task
- Encourages variety in activities
- Promotes balanced self-improvement
- Realistic time between similar activities

**What happens:**
1. You complete a specific task (e.g., "Do 20 push-ups")
2. Global cooldown starts (30 seconds - affects all tasks)
3. After global cooldown ends:
   - OTHER tasks become available
   - The task you just did shows **red timer badge**
4. Timer shows: **"⏰ 59m 30s"** (counting down)
5. Task button changes to gray **"Cooldown"** button
6. Timer updates every second showing remaining time
7. After 1 hour, task becomes available again

**Timer Display Formats:**
- **"59m 30s"** = 59 minutes, 30 seconds remaining
- **"45m 0s"** = 45 minutes exactly
- **"5m 15s"** = 5 minutes, 15 seconds
- **"45s"** = Just seconds when under 1 minute

**Visual Features:**
- Red rounded badge next to task name
- Clock icon (⏰) in badge
- Real-time countdown updates
- Task becomes semi-transparent
- Cooldown button is gray and disabled

**Technical Details:**
- Duration: 3,600,000 milliseconds (1 hour)
- Updates every 100ms for accuracy
- Each task tracked independently
- Cooldown persists if you close and reopen browser
- Stored in localStorage

### Cooldown Interaction Example

**Scenario:** You complete "Do 20 push-ups" at 10:00 AM

**10:00:00 AM** - Click Complete
- ✅ Receive 10 XP instantly
- 🔴 RED BANNER appears: "Refractory Period - Wait 30s"
- ⏸️ ALL tasks show "Wait" button
- 🏃 Push-ups task shows: "Cooldown" button

**10:00:30 AM** - Global cooldown expires
- ✅ Banner disappears
- 🟢 OTHER tasks show "Complete" button again
- ⏰ Push-ups task still shows: "59m 30s" timer
- 🎯 You can now do different tasks!

**11:00:00 AM** - Task cooldown expires
- ✅ Push-ups timer reaches 0
- 🟢 Push-ups "Complete" button returns
- 🎉 Can do push-ups again!

---

## Character Upgrades

### The Four Attributes

Your character has **four core attributes** that you can permanently upgrade using skill points. Each upgrade costs **1 skill point**.

### 💪 Physical Strength

**Description:** "Increases physical ability"

**Effects:**
- **Visual:** Muscles grow larger and more defined
- **Character Appearance:**
  - Arms get bigger and more muscular
  - Chest muscles (pecs) expand significantly
  - Abdominal muscles become visible (six-pack/eight-pack)
  - Overall body size increases
  - Biceps become prominent
  - Body scales up (max 50%+ larger)

**Recommended For:**
- If you focus on physical fitness
- Athletes and bodybuilders
- Those doing lots of exercise tasks
- Players who want impressive visual changes

**Level Progression:**
- Levels 1-5: Noticeable muscle growth
- Levels 6-10: Athletic/fit physique
- Levels 11-15: Bodybuilder appearance
- Levels 16+: Superhero-level musculature

**Best Tasks to Complement:**
- Daily: Exercise for 15 minutes
- Anytime: Do 20 push-ups, Intense workout

### ❤️ Endurance

**Description:** "Increases stamina and resilience"

**Effects:**
- **Visual:** Heart appears in chest and beats faster
- **Character Appearance:**
  - Red heart icon becomes visible
  - Heart beats with pulsing animation
  - Beat rate increases with more endurance
  - Heart becomes brighter and more prominent
  - Shows cardiovascular health

**Recommended For:**
- Endurance athletes (runners, cyclists)
- Those building stamina
- Players who want heart animation
- Focus on sustained physical activity

**Level Progression:**
- Levels 1-3: Heart appears, slow beat
- Levels 4-7: Heart beats faster, more visible
- Levels 8-12: Rapid heartbeat, bright red
- Levels 13+: Maximum cardiovascular display

**Best Tasks to Complement:**
- Daily: Exercise, Sleep 8 hours
- Anytime: Intense workout, Take a walk

### 🧠 Intelligence

**Description:** "Boosts learning and problem-solving"

**Effects:**
- **Visual:** Brain glows golden inside head
- **Character Appeara
