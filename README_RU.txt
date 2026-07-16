CLEARZONE ANDROID — установка

В архиве:
1. Полный проект Android Studio.
2. server/public/api/app_notifications.php — API уведомлений для сайта.

УСТАНОВКА API
Загрузите файл:
server/public/api/app_notifications.php
в папку сайта:
/public/api/app_notifications.php

Проверка:
после входа в игру откройте
https://clearzone.mobi/public/api/app_notifications.php
Должен вернуться JSON с authorized=true.

СБОРКА APK
1. Откройте папку ClearZone_Android_App в Android Studio.
2. Дождитесь Gradle Sync.
3. Build → Build APK(s).
4. APK: app/build/outputs/apk/debug/app-debug.apk

Работа уведомлений:
- при открытом приложении — проверка примерно раз в минуту;
- в фоне — системная проверка примерно раз в 15 минут;
- нажатие на уведомление открывает PDA → Диалоги;
- вход сохраняется через cookie сайта;
- пароль отдельно приложение не хранит.

Для мгновенных push-уведомлений требуется Firebase Cloud Messaging и google-services.json. Этот архив работает без Firebase.
