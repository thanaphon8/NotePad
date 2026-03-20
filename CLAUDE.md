# Daily Notepad Web App

> แอปพลิเคชันเว็บสำหรับจัดการงานประจำวัน ที่มีระบบ Gamification สไตล์ Duolingo

---

## Concept

A web application for managing daily tasks with a simple and engaging user experience inspired by **Duolingo**.

---

## User Flow

```
Open Website → Login / Register → Dashboard → Select Date
→ Add Task → Complete Task → Gain XP → View Progress
```

### Task Creation Flow
```
Click Add Task → Enter Text → Save → Display in List
```

### Task Completion Flow
```
Click Complete → Mark as Done → Add XP → Update Progress
```

---

## Core Features

- Add, edit, delete tasks
- Select date
- Mark task as completed
- Data storage (local storage or database)

---

## Gamification Features

- XP system
- Daily streak
- Progress bar
- Level system _(optional)_

---

## UI Design (Duolingo Style)

- **Primary color**: `#58CC02`
- Rounded buttons with shadow
- Button press animation

```css
.button {
  background-color: #58CC02;
  color: white;
  border-radius: 16px;
  box-shadow: 0 4px 0 #46A302;
}

.button:active {
  transform: translateY(4px);
  box-shadow: none;
}
```

---

## Pages Structure

| Page | Description |
|------|-------------|
| Dashboard | หน้าหลักแสดง tasks และ progress |
| Add Task Modal | Popup สำหรับเพิ่ม task ใหม่ |
| Calendar Page | เลือกและดู tasks ตามวันที่ |
| Profile Page | แสดง XP, streak และ level ของผู้ใช้ |

---

## Data Structure

### Task
```json
{
  "id": "number",
  "text": "string",
  "completed": "boolean",
  "date": "string"
}
```

### User
```json
{
  "username": "string",
  "xp": "number",
  "streak": "number"
}
```

---

## Development Steps

1. **Build UI** — HTML, CSS
2. **Add JavaScript logic**
3. **Use local storage**
4. **Build backend**
5. **Add gamification features**