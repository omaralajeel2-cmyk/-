# ألعب وأتعلم — تصميم عمر الرملي

## الطريقة 1: بناء APK تلقائيًا (بدون أي برنامج على جهازك)
1. أنشئ حسابًا مجانيًا على github.com ثم مستودعًا جديدًا (New repository).
2. ارفع كل محتويات هذا المجلد (Add file ← Upload files) بما فيها مجلد `.github` ومجلد `www`.
   - إن لم يُرفع `.github`: Add file ← Create new file، اكتب الاسم `.github/workflows/build-apk.yml` والصق فيه محتوى الملف.
3. افتح تبويب Actions ← Build APK ← Run workflow.
4. بعد 5 إلى 8 دقائق افتح التشغيل المكتمل ونزّل `kids-game-apk` (ملف zip فيه app-debug.apk).
5. انقل الملف للهاتف وثبّته (فعّل "التثبيت من مصادر غير معروفة" عند الطلب).

## الطريقة 2: على جهازك (Android Studio + Node.js)
npm install
npx cap add android
npx cap sync android
npx cap open android      # ثم Build ← Build APK(s)

## تعديل اللعبة
عدّل الملف www/index.html ثم أعد البناء.
