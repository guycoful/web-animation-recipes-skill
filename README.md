# web-animation-recipes

סקיל ל-Claude Code שמוסיף לאתר הנפשה אינטראקטיבית. כשטוענים אותו, הוא שואל איפה באתר לשים אותה, מתוך 8 מקומות: Hero, גלילה, כרטיסים, טפסים, כפתורים ומתגים, ניווט, הצגת מוצר ודמות שמלווה את הסמן. אם כבר כתבת את המקום בבקשה, הוא מדלג על השאלה. אחרי הבחירה הוא מציג רק את ההנפשות שמתאימות למקום, ושואל על הפלטפורמה, התוכן והדפדפנים לפני שהוא כותב קוד.

יש בו 30 מתכונים, ולכל אחד מפרט בנייה, טכנולוגיות מתאימות ופרמטרים לכיוונון. 10 מהם נשענים על API שזמין רק ב-Chrome, ובהם הסקיל מנחה לבנות חלופה לדפדפנים אחרים ולבדוק תמיכה בזמן ריצה.

התקנה:
```
git clone https://github.com/guycoful/web-animation-recipes-skill.git /tmp/web-animation-recipes
mkdir -p ~/.claude/skills/web-animation-recipes && cp /tmp/web-animation-recipes/{SKILL,placements,recipes}.md ~/.claude/skills/web-animation-recipes/
```
שימוש: כותבים לקלוד קוד "תוסיף הנפשה לאתר".
