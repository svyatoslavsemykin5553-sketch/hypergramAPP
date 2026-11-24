HYPERGRAM для Android — как получить APK без Android Studio

1. Зарегистрируйтесь на github.com и создайте новый репозиторий (можно Private).
2. Загрузите в него ВСЁ содержимое этой папки: Add file -> Upload files.
   Важно: должна загрузиться и скрытая папка .github (путь .github/workflows/build-apk.yml).
   Если она не загрузилась: Add file -> Create new file, в имени файла напишите
   .github/workflows/build-apk.yml и вставьте туда содержимое файла build-apk.yml.
3. Откройте вкладку Actions -> Build APK -> Run workflow. Сборка идёт 5-10 минут.
4. Откройте завершённый запуск, внизу в разделе Artifacts скачайте hypergram-apk (zip),
   внутри будет app-debug.apk. Перекиньте на телефон и установите
   (разрешите установку из неизвестных источников).

Обновление приложения: замените файл www/index.html новой версией сайта
и снова запустите Build APK. Сайт и приложение используют одну и ту же базу.
