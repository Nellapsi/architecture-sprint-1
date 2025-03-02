Для разделение на микрофронтенды был выбран подход Webpack Module Federation
Данный подход был выбран по причине использования одного фреймворка для всех микрофронтендов, которые могут использовать одну кодовую базу и не нуждаются в отдельном вызове страниц как в Single SPA
Фронтенд был разделен на 6 частей:
1. host - объединяет все микрофронтеды по подходу Webpack Module Federation
2. card - фронденд отвечающий за отображение карточек с путешествиями
3. editUser - отвечает за редактирование профиля пользователя
4. register - отвечает за регистрацию и авторизацию пользователя
5. genetal - собирает в себе все части необходимые для каждой страницы (шапка, подвал, ошибки) 
6. addPlacePopup - отвечает за добавление картинок в приложение
При корректной настройке за запуск приложения отвечал бы файл compose.yaml и файлы докера:
1. Dockerfile.host
2. Dockerfile.card
3. Dockerfile.editUser
4. Dockerfile.register
5. Dockerfile.genetal
6. Dockerfile.addPlacePopup
7. Dockerfile.backend

второе задание: https://drive.google.com/file/d/1NZb7o1NUvxZ5fp1ezyxfa4wOAgKRQeR_/view?usp=drive_link