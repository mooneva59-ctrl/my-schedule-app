ПРОЕКТ «МОЁ РАСПИСАНИЕ» — Android APK + сайт

В проекте есть:
- Android-приложение на WebView;
- сборка APK через GitHub Actions;
- публикация сайта расписания через GitHub Pages.

ВАЖНО: Android-приложение загружает страницу расписания с GitHub Pages, поэтому интернет нужен для открытия расписания. Изменения хранятся в локальном хранилище WebView на этом устройстве. Перед очисткой данных приложения экспортируйте JSON-резервную копию.

КАК УСТАНОВИТЬ ПРОЕКТ В РЕПОЗИТОРИЙ:
1. Распакуйте архив.
2. Загрузите ВСЁ содержимое папки проекта в корень репозитория my-schedule-app (включая скрытую папку .github).
3. Не удаляйте ваш исходный index.html и README.txt — они нужны сайту.
4. На GitHub откройте Settings → Pages и в разделе Build and deployment выберите Source: GitHub Actions.
5. Откройте вкладку Actions. Должны запуститься два процесса: Build Android APK и Publish schedule website.

ГДЕ ЗАБРАТЬ APK:
Actions → успешный запуск Build Android APK → Artifacts → moe-raspisanie-apk.
Скачанный ZIP содержит app-debug.apk. Распакуйте его и откройте APK на Android для установки.

Если Actions не запускаются, проверьте Settings → Actions → General и разрешение GitHub Actions для репозитория.
