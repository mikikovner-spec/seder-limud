# סדר הלימוד היומי

אפליקציית ווב למעקב יומי אחר סדר הלימוד: אשף הגדרות, צ'קליסט יומי עם שיעורים לפי לוח, השלמות בדיעבד ודשבורד.
הנתונים נשמרים בדפדפן של כל משתמש (localStorage). אין שרת ואין משתמשים.

## העלאה ל-GitHub Pages
1. ב-github.com: New repository, שם למשל `seder-limud`, מסוג Public.
2. Add file → Upload files, וגוררים את כל הקבצים שבתיקייה הזו. Commit changes.
3. Settings → Pages → Build and deployment → Source: Deploy from a branch, Branch: `main`, תיקייה `/ (root)` → Save.
4. אחרי דקה-שתיים האפליקציה זמינה בכתובת `https://<שם-המשתמש>.github.io/seder-limud/`.

## עדכון גרסה
מעלים מחדש את `app.js` (ושאר הקבצים שהשתנו), ומעלים את המספר ב-`CACHE` שבקובץ `sw.js` (למשל ל-`seder-limud-v2`), כדי שהטלפונים יקבלו את הגרסה החדשה.

## קוד המקור
התיקייה `src` בקובץ המלא מכילה את קוד המקור. `app.js` נבנה ממנה עם `npm install && npm run build`.
את הדף של ליקוטי הלכות מגדירים בקובץ `src/portions.js` (המשתנה `LH`): תאריך עוגן, מספר הדף באותו יום, והדף האחרון בכרך.
