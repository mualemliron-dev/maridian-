# 🪐 Meridian Performance Galaxy

> פלטפורמת HR analytics ויזואלית שממירה נתוני ביצועי עובדים לגלקסיה אינטראקטיבית — כל עובד הוא כוכב.

**Version:** 17 | **Date:** June 2026 | **Status:** Live

🔗 **Live Demo:** [meridian-galaxy.vercel.app](https://meridian-galaxy.vercel.app)
📄 **PRD:** [PRD.md](./PRD.md)
✅ **Tasks:** [tasks.md](./tasks.md)

---

## 📖 תיאור הפרויקט

Meridian Performance Galaxy הוא דשבורד HR ויזואלי שבו כל עובד מיוצג ככוכב המקיף שמש מרכזית. המיקום, הגודל, הצבע והטבעת של כל כוכב מקודדים ממדי ביצועים שונים בו-זמנית:

| מאפיין ויזואלי | משמעות |
|---|---|
| גודל כוכב | ציון ביצועים (0–100) |
| רדיוס מסלול | ותק בשנים |
| צבע כוכב | מחלקה ארגונית |
| טבעת זהב | עובד מצטיין (Excellence) |
| קווים מקווקווים | חיבור בין מצטיינים |

---

## 🚀 הרצה מקומית

### דרישות מקדימות
- דפדפן מודרני (Chrome / Firefox / Safari / Edge)
- אין צורך ב-Node.js, npm, או build tools כלשהם

### התקנה והרצה

```bash
# שיבוט ה-repository
git clone https://github.com/YOUR_USERNAME/meridian-galaxy.git

# כניסה לתיקייה
cd meridian-galaxy

# פתיחה ישירה בדפדפן
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux

# או הרצה עם שרת מקומי (מומלץ)
npx serve .
# ואז פתיחת http://localhost:3000
```

### אין צורך ב-build
הפרויקט הוא קובץ HTML יחיד (`index.html`) ללא תלויות חיצוניות. פתיחה ישירה בדפדפן עובדת מיידית.

---

## 🗂️ מבנה הפרויקט

```
meridian-galaxy/
├── index.html      # כל הפרויקט — HTML + CSS + JS בקובץ אחד
├── PRD.md          # מסמך אפיון המוצר
├── tasks.md        # תוכנית עבודה עם היסטוריית התקדמות
└── README.md       # המסמך הזה
```

---

## 📊 הנתונים

### מקור
הנתונים **מקומיים בלבד** — מוטמעים ישירות ב-`index.html` כמערך JavaScript. אין API חיצוני, אין מסד נתונים, אין קריאות רשת.

### עובדים (13 כוכבים)

| שם | תפקיד | מחלקה | ציון | ותק | מצטיין | בונוס |
|---|---|---|---|---|---|---|
| Inon Katz | Data Security | Data Security | 100 | 3 | ✅ | ₪70K |
| Michelle Levy | Head of Sales | Engineering | 99 | 5 | ✅ | ₪28K |
| Jonathan Cohen | Lead Engineer | Engineering | 90 | 4 | ✅ | ₪24K |
| Tamar Shapiro | Product Designer | Design | 90 | 3 | ✅ | ₪20K |
| Ori Goldberg | Product Manager | Product | 87 | 2 | ❌ | ₪18K |
| Noa Ben-David | HR Manager | HR | 85 | 6 | ❌ | ₪17K |
| Avi Mizrahi | Security Engineer | Security | 83 | 1 | ❌ | ₪16K |
| Shira Peretz | Data Analyst | Data | 82 | 3 | ❌ | ₪16K |
| Yael Katz | Frontend Dev | Engineering | 80 | 2 | ❌ | ₪15K |
| Dan Friedman | UX Designer | Design | 79 | 1 | ❌ | ₪14K |
| Liora Stern | Backend Dev | Engineering | 77 | 4 | ❌ | ₪14K |
| Matan Levi | Data Scientist | Data | 75 | 2 | ❌ | ₪13K |
| Hila Avraham | Product Analyst | Product | 72 | 1 | ❌ | ₪12K |

### הוספת עובד חדש
ערוך את מערך `EMPLOYEES` ב-`index.html`:

```javascript
{
  id: 13,
  name: "שם העובד",
  role: "תפקיד",
  dept: "Engineering",  // חייב להתאים ל-DEPT_COLORS
  score: 85,            // 0–100
  tenure: 2,            // שנים
  excellence: false,
  bonus: 20             // ₪K
}
```

---

## 🎮 מדריך שימוש

| פעולה | תוצאה |
|---|---|
| גרירה אופקית | סיבוב הגלקסיה |
| גלגלת עכבר | זום פנימה/החוצה |
| Hover על כוכב | Tooltip עם פרטים |
| לחיצה על כוכב | פתיחת פאנל פרטי עובד |
| לחיצה על שורה ב-Leaderboard | בחירת עובד + camera pan |
| כפתור Export | שמירת PNG של הגלקסיה |

---

## ⚠️ מגבלות ובאגים ידועים

| # | תיאור | חומרה |
|---|---|---|
| BUG-01 | ב-Safari ישן (< 15) backdrop-filter לא נתמך | נמוכה |
| BUG-02 | במסכים צרים מ-1280px ה-Header נחתך | בינונית |
| BUG-03 | ייצוא PNG כולל רק את ה-canvas, לא את ה-UI | By Design |
| LIM-01 | הנתונים hardcoded — אין API חיצוני | Out of Scope v17 |
| LIM-02 | לא מותאם למסכי מגע / מובייל | Out of Scope v17 |

---

## 🛠️ Stack טכני

- **HTML5 Canvas 2D API** — רינדור הגלקסיה
- **Vanilla JavaScript (ES6+)** — לוגיקה ואינטראקציה
- **CSS3** — עיצוב ו-glassmorphism
- **Vercel** — hosting סטטי
- **ללא frameworks, ללא תלויות חיצוניות**

---

*Meridian Performance Galaxy — Built with Vanilla JS*
