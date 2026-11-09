# מתכונים: 30 הנפשות

לכל מתכון: מה רואים, מפרט לבנייה באנגלית (לסוכן הקוד), טכנולוגיות מתאימות וכפתורי כיוונון לחשיפה בממשק. המימוש נבנה מאפס.


## Liquid Tags (liquid-tags)
- מיקומים מתאימים: כפתורים, מתגים ומחווני התקדמות
- מה רואים: מחוון התקדמות מזכוכית, שהשלבים בו נמשכים זה לזה ומתמזגים כמו נוזל.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GLSL shader, SDF, WebGL, glass/refraction
- Build spec: Five-step progress indicator rendered in one WebGL2 fragment shader using signed distance fields. Each step is a smooth glass pill over a photo background, refracting it with slight per-channel dispersion and frosting. Filling moves as one continuous liquid front; neighbouring pills grow small magnetic bulges toward each other and merge when the front reaches them.
- כפתורי כיוונון מוצעים: IOR, עובי, dispersion, frost, מהירות, עוצמה, צבעים, רעש

## Glass Light Toggle (glass-light-toggle)
- מיקומים מתאימים: כפתורים, מתגים ומחווני התקדמות
- מה רואים: מתג מצב כהה ובהיר עם ידית זכוכית ופס אור שמסתובב סביבה.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GLSL shader, WebGL, glass/refraction
- Build spec: Light/dark switch drawn in a single fragment shader. The knob is a rounded-square glass lens whose bevel refracts and frosts the track beneath it, with mild chromatic aberration. A strip of light orbits the knob while switching (bottom at night, top by day), scattering into the glass and spilling onto the page. While dragging, the icon is rebuilt pixel by pixel from moon to sun.
- כפתורי כיוונון מוצעים: IOR, עובי, dispersion, frost, מהירות, עוצמה, צבעים, רעש

## Lathe Blueprint (lathe-blueprint)
- מיקומים מתאימים: אזור הפתיחה (Hero) של דף נחיתה
- מה רואים: Hero של חברת חומרה: שרטוט טכני שמצייר את עצמו וחושף את המוצר האמיתי.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GLSL shader, Three.js, WebGL
- Build spec: Hero where a technical line drawing animates itself in, then a square-by-square mask reveals the real product render underneath on hover. On click the page tilts into 3D (Three.js, fixed sun light, real shadows): a drone model lifts off and follows the cursor, its rotor wash bending the page surface locally and pushing extruded headline letters around.
- כפתורי כיוונון מוצעים: מהירות, עוצמה, צבעים, רעש, FOV, מרחק מצלמה, תאורה

## One Time Code (one-time-code)
- מיקומים מתאימים: טפסים, שדות קלט וקוד חד-פעמי
- מה רואים: כרטיס עם קוד הפעלה שנשרף אחרי שראו אותו.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: Canvas, GLSL shader, WebGL
- Build spec: An HTML card showing a one-time code that burns away after reveal. A GPU fluid simulation (air, fuel, combustion) runs on top, charring the surface, burning holes and shedding curled glowing flakes the cursor can blow around. Where HTML-in-canvas is unsupported, swap to a static snapshot of the card once the reveal finishes.
- כפתורי כיוונון מוצעים: מהירות, עוצמה, צבעים, רעש

## Liquid Glass Recorder (liquid-glass-recorder)
- מיקומים מתאימים: טפסים, שדות קלט וקוד חד-פעמי; כפתורים, מתגים ומחווני התקדמות
- מה רואים: כפתור הקלטה קולית מזכוכית נוזלית שנמשך לסמן וזוהר כשמדברים.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GLSL shader, Web Audio, WebGL
- Build spec: Voice/record button for AI apps. A refracting glass slab with a spring-driven liquid shape that leans toward the pointer, and a glow driven by several frequency bands of microphone input while recording. Expose many tuning parameters.
- כפתורי כיוונון מוצעים: מהירות, עוצמה, צבעים, רעש, רגישות מיקרופון, מספר פסים

## Aphelion (aphelion)
- מיקומים מתאימים: אזור הפתיחה (Hero) של דף נחיתה
- מה רואים: דף השקה מלא: אסטרונאוט נופל ליד כוכב לכת מוסתר בזמן הגלילה.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GSAP, Three.js, scroll-driven
- Build spec: Full responsive launch page around a live 3D scene: a rigged astronaut drifting in freefall in front of an eclipsed planet with a slowly shifting glow. Scroll drives the camera and astronaut via GSAP ScrollTrigger. Vite + Three.js, self-hosted fonts.
- כפתורי כיוונון מוצעים: אורך גלילה לכל שלב, easing, משך, stagger, easing, FOV, מרחק מצלמה, תאורה

## Cephalopod (cephalopod)
- מיקומים מתאימים: דמות או אפקט שמלווה את הסמן בכל הדף
- מה רואים: יצור ימי שמשוטט בדף ועוקב אחרי הסמן.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GLSL shader, React Three Fiber, Three.js
- Build spec: An organic creature (marching-cubes body) that explores the page and follows the cursor. Offer several switchable material looks: PBR with environment lighting, matcap, parallax height maps, transmission, and screen-space subsurface scattering.
- כפתורי כיוונון מוצעים: מהירות, עוצמה, צבעים, רעש, FOV, מרחק מצלמה, תאורה

## Vine Overgrowth (vine-overgrowth)
- מיקומים מתאימים: אזור הפתיחה (Hero) של דף נחיתה; דמות או אפקט שמלווה את הסמן בכל הדף
- מה רואים: גפנים חיים שגדלים על דף נחיתה בתנועה ונמשכים לסמן.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GLSL shader, React Three Fiber, Three.js, particles
- Build spec: A band of bricks moving along curved 3D tracks while procedural braided vines grow over it, their tips leaning toward the cursor. Bricks passing a growth zone get covered in moss and instanced plant clumps behind a noisy growth front, all grounded by a contact shadow.
- כפתורי כיוונון מוצעים: כמות חלקיקים, גודל, אורך חיים, צפיפות, מהירות, עוצמה, צבעים, רעש, FOV, מרחק מצלמה, תאורה

## Surface Dissolve (surface-dissolve)
- מיקומים מתאימים: מעבר בגלילה או מעבר בין מסכים
- מה רואים: דף נחיתה שמתקפל כמו נייר ומתפוגג לעשן בגלילה.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: GLSL shader, HTML-in-Canvas (experimental), Three.js, particles, scroll-driven
- Build spec: The landing page is rendered onto a 3D sheet that curls as you scroll; inside a height band it dissolves into smoke: a GPU particle system releases page pixels as grains along a soft, wandering erosion front. Pointer input is ray-mapped onto the deformed sheet so form fields stay usable.
- כפתורי כיוונון מוצעים: אורך גלילה לכל שלב, easing, כמות חלקיקים, גודל, אורך חיים, צפיפות, מהירות, עוצמה, צבעים, רעש, FOV, מרחק מצלמה, תאורה
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Dot Sphere Card (dot-sphere-card)
- מיקומים מתאימים: כרטיסים ורשת פיצ'רים
- מה רואים: כרטיס מדע בדיוני עם כדור נקודות שמסתובב אחרי הסמן.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: CSS 3D, Canvas, Three.js
- Build spec: Futuristic HUD card in CSS 3D: a dot sphere that rotates to face the cursor floats over a tinted video layer. On hover, two 3D asteroid models orbit out from behind the card with real shadows and a cursor-tracking spotlight; each layer has its own reveal timing. Dither the background to avoid gradient banding.
- כפתורי כיוונון מוצעים: FOV, מרחק מצלמה, תאורה

## Glass Hero (glass-hero)
- מיקומים מתאימים: אזור הפתיחה (Hero) של דף נחיתה
- מה רואים: Hero מאחורי רסיסי זכוכית אמיתיים ששוברים את האור לצבעים.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: HTML-in-Canvas (experimental), React Three Fiber, Three.js, glass/refraction
- Build spec: Live HTML hero behind floating glass shapes that refract it with chromatic dispersion (Three.js MeshPhysicalMaterial: IOR, thickness, dispersion). Shapes can be dragged; expose the glass parameters in a tuning panel.
- כפתורי כיוונון מוצעים: IOR, עובי, dispersion, frost, FOV, מרחק מצלמה, תאורה
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Jungle Cursor Canopy (jungle-cursor-canopy)
- מיקומים מתאימים: אזור הפתיחה (Hero) של דף נחיתה; דמות או אפקט שמלווה את הסמן בכל הדף
- מה רואים: סבך ג'ונגל צפוף שנפתח סביב הסמן ואז מתרומם.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GLSL shader, GSAP, Three.js, particles
- Build spec: Dense procedural leaf canopy covering the page that parts around the cursor, then lifts and spirals past the camera in a choreographed GSAP intro. Leaves use generated silhouettes, physical materials, wind gusts and depth of field, with floating glowing particles.
- כפתורי כיוונון מוצעים: כמות חלקיקים, גודל, אורך חיים, צפיפות, מהירות, עוצמה, צבעים, רעש, משך, stagger, easing, FOV, מרחק מצלמה, תאורה

## Pendant Lamp (pendant-lamp)
- מיקומים מתאימים: אזור הפתיחה (Hero) של דף נחיתה
- מה רואים: מנורה תלויה שמאירה דף כהה, ואפשר לתפוס ולזרוק אותה.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: Canvas, React Three Fiber, Three.js, WebGL, physics
- Build spec: A pendant lamp on a physical pendulum lights the page. Outside the light cone the page is shown in a dark treatment (grayscale + blur, outline, halftone, CRT or dither); inside the cone the real page shows. The lamp can be grabbed and thrown; hovering a button aims the beam at it.
- כפתורי כיוונון מוצעים: כבידה, ריסון, משקל, FOV, מרחק מצלמה, תאורה
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Action Wheel (action-wheel)
- מיקומים מתאימים: ניווט ותפריטים
- מה רואים: תפריט רדיאלי כמו במשחקים: לוחצים ומחזיקים, מכוונים לפעולה ומשחררים.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GLSL shader, React Three Fiber, Three.js
- Build spec: Press-and-hold radial menu: an animated noise dot grid, a segmented ring with variable stroke, and four quadrants that light up as a glow follows the pointer around the rim. The wheel tilts in 3D toward the cursor; releasing over a quadrant confirms the action.
- כפתורי כיוונון מוצעים: מהירות, עוצמה, צבעים, רעש, FOV, מרחק מצלמה, תאורה

## Cuboid Chain (cuboid-chain)
- מיקומים מתאימים: כרטיסים ורשת פיצ'רים; הצגת מוצר או אפליקציה (מוקאפ טלפון, קרוסלה)
- מה רואים: שורת קוביות תלת ממדיות שמתגלגלות בגל, ועל כל פאה כרטיס מוצר.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: React Three Fiber, Three.js
- Build spec: Horizontal row of rounded cuboids, each face carrying a product/task card image. Each cuboid rolls around the horizontal axis with a staggered phase, lit by key lights from top, bottom and side. Expose size, gap, speed, stagger and lights.
- כפתורי כיוונון מוצעים: זווית הטיה מקסימלית, עומק, מספר שכבות, עוצמת אורות, צבע, כיוון, FOV, מרחק מצלמה, תאורה

## Trace Cards (trace-cards)
- מיקומים מתאימים: כרטיסים ורשת פיצ'רים
- מה רואים: כרטיסים שנוטים לכיוון הסמן ומשאירים אחריהם עותקים זוהרים.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: React Three Fiber, Three.js
- Build spec: Cards with cursor-driven tilt and depth that emit a stream of trailing duplicate layers as they move (pyramid/diamond formations). 3D layer over normal HTML chrome.
- כפתורי כיוונון מוצעים: זווית הטיה מקסימלית, עומק, מספר שכבות, FOV, מרחק מצלמה, תאורה

## Pattern Cards (pattern-cards)
- מיקומים מתאימים: כרטיסים ורשת פיצ'רים
- מה רואים: שלושה כרטיסי פיצ'רים בולטים עם איור נקודות.
- מורכבות: נמוך (CSS/HTML)
- טכנולוגיות מתאימות: HTML/CSS
- Build spec: Three tall feature cards in strong contrasting colours, each with its own dot-pattern illustration and a title in the bottom corner. Static layout, pure HTML/CSS (or SVG for the patterns).
- כפתורי כיוונון מוצעים: זווית הטיה מקסימלית, עומק, מספר שכבות

## Twisting Ribbons (twisting-ribbons)
- מיקומים מתאימים: כרטיסים ורשת פיצ'רים
- מה רואים: שורת סרטים צרים שמתפתלים ברצף ויוצרים צורות ברווחים ביניהם.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: GLSL shader, React Three Fiber, Three.js
- Build spec: A row of thin vertical ribbons, each rotated a bit more around its Y axis from left (edge-on) to right (face-on and beyond). A band along each ribbon blends two materials, and the gaps between neighbours form lens-shaped negative spaces.
- כפתורי כיוונון מוצעים: מהירות, עוצמה, צבעים, רעש, FOV, מרחק מצלמה, תאורה

## Dot Form (dot-form)
- מיקומים מתאימים: טפסים, שדות קלט וקוד חד-פעמי
- מה רואים: טופס שקופץ לתלת ממד בלחיצה, והאותיות עולות משדה של נקודות.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: HTML-in-Canvas (experimental), React Three Fiber, Three.js
- Build spec: On focus, a standard form lifts into a tilted 3D scene: input and checkbox become extruded outlines, the button gains depth, and typed characters appear as raised dots at varying heights. Keep a normal 2D form as fallback.
- כפתורי כיוונון מוצעים: משך המעבר, easing, FOV, מרחק מצלמה, תאורה
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Shader Deck (shader-deck)
- מיקומים מתאימים: מעבר בגלילה או מעבר בין מסכים; הצגת מוצר או אפליקציה (מוקאפ טלפון, קרוסלה)
- מה רואים: שקופיות שמסתובבות דרך שער זוהר בזמן הגלילה.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: GLSL shader, HTML-in-Canvas (experimental), React Three Fiber, Three.js
- Build spec: 3D carousel of HTML slides on a ring that scroll through a glowing portal plane, with volumetric light, fog, bloom and chromatic aberration (R3F + drei).
- כפתורי כיוונון מוצעים: מהירות, עוצמה, צבעים, רעש, מספר שקופיות, מהירות, רדיוס, FOV, מרחק מצלמה, תאורה
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Code Slice Hero (code-slice-hero)
- מיקומים מתאימים: אזור הפתיחה (Hero) של דף נחיתה
- מה רואים: דף נחיתה שמתנפץ לאריחים וחושף מתחתיו טרמינל חי.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: GLSL shader, HTML-in-Canvas (experimental), React Three Fiber, Three.js
- Build spec: Landing page that hovers, lifts and breaks into a grid of tiles that fly apart to reveal a document view and a working terminal underneath.
- כפתורי כיוונון מוצעים: מהירות, עוצמה, צבעים, רעש, FOV, מרחק מצלמה, תאורה
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Dot Phone Carousel (dot-phone-carousel)
- מיקומים מתאימים: הצגת מוצר או אפליקציה (מוקאפ טלפון, קרוסלה)
- מה רואים: מסכים מחליקים מאחורי טלפון ונסרקים לתוכו בדפדוף.
- מורכבות: בינוני (Canvas 2D)
- טכנולוגיות מתאימות: Canvas
- Build spec: Centered phone mockup with a sharp screen while dotted preview images slide behind it in a horizontal carousel. Moving left/right pulls each image through the phone with a scan-line transition.
- כפתורי כיוונון מוצעים: מספר שקופיות, מהירות, רדיוס, משך המעבר, easing

## Cursor Nav (cursor-nav)
- מיקומים מתאימים: ניווט ותפריטים
- מה רואים: לחיצה הופכת את הסמן לתפריט תלת ממדי שמנווטים בו בתנועה למעלה ולמטה.
- מורכבות: נמוך (CSS/HTML)
- טכנולוגיות מתאימות: HTML/CSS
- Build spec: A custom cursor behaves normally, then on click expands into a 3D navigation mode; moving up and down steers the selection, release to choose.
- כפתורי כיוונון מוצעים: משך המעבר, easing

## Particle Phones (particle-phones)
- מיקומים מתאימים: מעבר בגלילה או מעבר בין מסכים; הצגת מוצר או אפליקציה (מוקאפ טלפון, קרוסלה)
- מה רואים: ענן חלקיקים שמתגבש לכל מסך טלפון חדש בזמן הגלילה.
- מורכבות: בינוני (Canvas 2D)
- טכנולוגיות מתאימות: Canvas, particles, scroll-driven
- Build spec: Three-column scroll page. The middle column holds drifting particles; as each section headline arrives, the particles snap into a phone screenshot, then dissolve again for the next one (Canvas 2D).
- כפתורי כיוונון מוצעים: אורך גלילה לכל שלב, easing, כמות חלקיקים, גודל, אורך חיים, צפיפות

## Dot Hover Cards (dot-hover-cards)
- מיקומים מתאימים: כרטיסים ורשת פיצ'רים
- מה רואים: דף שמצויר כולו בנקודות: ריחוף מאיר כרטיס, ולחיצה מביאה אותו לפוקוס.
- מורכבות: בינוני (Canvas 2D)
- טכנולוגיות מתאימות: Canvas
- Build spec: Whole page drawn as a grid of grey dots. Hovering a card region turns its dots white to reveal the card silhouette; clicking transitions the dots smoothly into the real, sharp HTML card.
- כפתורי כיוונון מוצעים: משך המעבר, easing

## Curtain Sidebar (curtain-sidebar)
- מיקומים מתאימים: ניווט ותפריטים
- מה רואים: מקלפים את הדף מהקצה השמאלי כמו נייר כדי לחשוף את סרגל הצד.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: Canvas, WebGL
- Build spec: Dragging from the left edge folds the page back like paper (curtain deformation in WebGL), revealing the sidebar underneath.
- כפתורי כיוונון מוצעים: לפי התוכן
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Mobius Strip (mobius-strip)
- מיקומים מתאימים: מעבר בגלילה או מעבר בין מסכים
- מה רואים: דף נחיתה שעטוף על טבעת מוביוס, וגוללים כדי לנוע לאורכה.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: Canvas, WebGL
- Build spec: The landing page content is mapped onto a 3D Möbius strip; scrolling rotates the strip so the reader travels along the content.
- כפתורי כיוונון מוצעים: לפי התוכן
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Shader Cards (shader-cards)
- מיקומים מתאימים: מעבר בגלילה או מעבר בין מסכים
- מה רואים: דף נחיתה שמתרכב מחלקיקים מעופפים בזמן הגלילה.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: Canvas, GLSL shader, WebGL
- Build spec: Scrollable page rendered to canvas while particles rain down and collide with page elements, using a brightness-based collision map so they settle on text and shapes.
- כפתורי כיוונון מוצעים: מהירות, עוצמה, צבעים, רעש
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Html In Canvas (html-in-canvas)
- מיקומים מתאימים: דמות או אפקט שמלווה את הסמן בכל הדף
- מה רואים: שער שעוקב אחרי הסמן וחושף ממשק נקי בתוך שדה חלקיקים.
- מורכבות: ניסיוני (Chrome בלבד)
- טכנולוגיות מתאימות: Canvas, WebGL
- Build spec: A cursor-following portal reveals a clean interface inside a particle field. Built on rendering real HTML into canvas (experimental drawElementImage), which also enables wave, kaleidoscope, shatter, melt and glitch shader effects on live UI.
- כפתורי כיוונון מוצעים: לפי התוכן
- תאימות: נשען על HTML-in-Canvas (WICG drawElementImage), שזמין רק ב-Chrome. חובה לבנות fallback, למשל צילום של ה-HTML כטקסטורה או גרסת CSS, ולבדוק תמיכה בזמן ריצה.

## Viewport Transition (viewport-transition)
- מיקומים מתאימים: מעבר בגלילה או מעבר בין מסכים
- מה רואים: דף שיווקי שטוח שנפתח לעולם תלת ממדי של קווים זוהרים.
- מורכבות: גבוה (WebGL/Three.js/שיידרים)
- טכנולוגיות מתאימות: Three.js
- Build spec: A flat 2D marketing page transforms into an immersive 3D wireframe scene with extruded text, bloom and chromatic aberration.
- כפתורי כיוונון מוצעים: משך המעבר, easing, FOV, מרחק מצלמה, תאורה
