# Дурак — Android-додаток

## Спосіб 1: без комп’ютера (APK в хмарі)
1. Створіть безкоштовний акаунт на github.com і новий репозиторій.
2. Завантажте в нього весь вміст цієї папки (Add file → Upload files; папка `.github` має потрапити теж).
3. Відкрийте вкладку Actions → Build APK → Run workflow.
4. Через 3–5 хвилин відкрийте завершений запуск і скачайте `durak-apk` (zip з `app-debug.apk`).
5. Розпакуйте, перекиньте на телефон і встановіть (дозвольте встановлення з невідомих джерел).

## Спосіб 2: на комп’ютері
Потрібні Node.js 20+, Java 17 та Android Studio.
    npm install
    npx cap add android
    npx cap sync android
    npx cap open android   # Build → Build APK(s)

## Іконка
`resources/icon.svg` — вихідник іконки. Щоб застосувати: `npm i -D @capacitor/assets`, перетворіть SVG на `resources/icon.png` (1024×1024) і виконайте `npx capacitor-assets generate --android`.
