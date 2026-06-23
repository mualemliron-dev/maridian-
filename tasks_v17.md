# tasks.md — תוכנית עבודה: Meridian Performance Galaxy
**Version:** 17
**Date:** June 2026
**כלל אצבע:** משימה אחת ≈ commit אחד

---

## שלב 1 — תשתית ומבנה בסיסי

- [x] **TASK-01** — יצירת `index.html` עם מבנה HTML בסיסי ו-CSS reset
  - _commit: `init: project scaffold and base HTML structure`_

- [x] **TASK-02** — הגדרת מערך נתוני העובדים (EMPLOYEES) + palette צבעים לפי מחלקה
  - _commit: `data: add employees dataset and department color palette`_

- [x] **TASK-03** — בניית Header עם לוגו ו-KPI bar
  - _commit: `feat: header component with KPI bar`_

---

## שלב 2 — מנוע הגלקסיה

- [x] **TASK-04** — הוספת Canvas ל-full viewport + render loop עם `requestAnimationFrame`
  - _commit: `feat: canvas setup and animation loop`_

- [x] **TASK-05** — רינדור שדה כוכבים רקע (300+ נקודות) עם נצנוץ
  - _commit: `feat: starfield background with twinkling`_

- [x] **TASK-06** — רינדור שמש מרכזית עם radial gradient glow
  - _commit: `feat: central sun with glow layers`_

- [x] **TASK-07** — רינדור כוכבי עובדים על מסלולים אליפטיים — גודל לפי ציון, צבע לפי מחלקה
  - _commit: `feat: employee stars on elliptical orbits`_

- [x] **TASK-08** — טבעת זהב למצטיינים + קווים מקווקווים בין מצטיינים
  - _commit: `feat: excellence ring and excellence links`_

---

## שלב 3 — אינטראקציה

- [x] **TASK-09** — Drag לסיבוב + Scroll לזום
  - _commit: `feat: drag to rotate and scroll to zoom`_

- [x] **TASK-10** — Hover detection + tooltip עם פרטי עובד
  - _commit: `feat: star hover detection and tooltip`_

- [x] **TASK-11** — לחיצה על כוכב → בחירה + camera pan
  - _commit: `feat: click to select star and camera follow`_

---

## שלב 4 — Leaderboard

- [x] **TASK-12** — בניית Leaderboard עם מיון לפי ציון
  - _commit: `feat: leaderboard panel with score ranking`_

- [x] **TASK-13** — Tabs למיון לפי Score / Tenure / Bonus
  - _commit: `feat: leaderboard sort tabs`_

- [x] **TASK-14** — Hover על שורה → הדגשת כוכב; לחיצה → בחירה
  - _commit: `feat: leaderboard row interaction`_

---

## שלב 5 — פאנל פרטי עובד

- [x] **TASK-15** — Employee Detail Panel עם אווטאר ופרטים
  - _commit: `feat: employee detail panel component`_

- [x] **TASK-16** — Performance bar ויזואלי + כפתור סגירה
  - _commit: `feat: performance bar and close button`_

---

## שלב 6 — חיפוש, סינון ו-Minimap

- [x] **TASK-17** — Sector Map (minimap) בזמן אמת
  - _commit: `feat: sector map minimap`_

- [x] **TASK-18** — חיפוש חי לפי שם / תפקיד / מחלקה + עמעום
  - _commit: `feat: live search with dimming`_

- [x] **TASK-19** — כפתורי סינון לפי מחלקה (auto-generated)
  - _commit: `feat: department filter buttons`_

---

## שלב 7 — Deploy ותיעוד

- [x] **TASK-20** — העלאה ל-GitHub repository
  - _commit: `chore: push to GitHub`_

- [x] **TASK-21** — חיבור ל-Vercel ו-deploy
  - _commit: `chore: Vercel deployment`_

- [x] **TASK-22** — כתיבת `PRD.md`
  - _commit: `docs: add PRD`_

- [x] **TASK-23** — כתיבת `tasks.md`
  - _commit: `docs: add tasks plan`_

- [ ] **TASK-24** — כתיבת `README.md` מלא
  - _commit: `docs: add README`_

- [ ] **TASK-25** — בדיקות קצה-לקצה: חיפוש, סינון, ייצוא, פאנל
  - _commit: `test: end-to-end QA pass`_

---

## סטטוס כללי

| שלב | משימות | הושלמו |
|---|---|---|
| 1 — תשתית | 3 | ✅ 3/3 |
| 2 — גלקסיה | 5 | ✅ 5/5 |
| 3 — אינטראקציה | 3 | ✅ 3/3 |
| 4 — Leaderboard | 3 | ✅ 3/3 |
| 5 — Detail Panel | 2 | ✅ 2/2 |
| 6 — חיפוש וסינון | 3 | ✅ 3/3 |
| 7 — Deploy ותיעוד | 6 | 🔄 4/6 |
| **סה"כ** | **25** | **23/25** |
