________________________________________________
Для хостинга на shneider-host.ru
________________________________________________

1) делаем zip
2) заливаем zip в ‘public html’
3) распаковываем и удаляем папку ‘mac’
4) переносим содержимое папки ‘public’ в ‘solution25’
5) переносим содержимое ‘solution25’ в ‘public html’
6) настраиваем ссылки (если в layout/index.html они не настроены или настроены на github) как тут ‘href="http://solution25.ru/css/bootstrap.min.css” ’

Для того, чтобы не было подтверждения о успешной отправке письма из формы, делаем в форме скрытое поле 
                     <input type="hidden" name="_next" value="http://solution25.ru">
Так же пытаемся скрыть ящик от спам-бота
                     <input type="text" name="_gotcha" style="display:none">



________________________________________________
Для хостинга на github.com
________________________________________________

1) создаем новый репозиторий
2) в config файле прописываем baseurl как https://<username>.github.io/<projectname>.github.io/public/
3) выполняем команду ‘ hugo ’ в папке с проектом
4) выполняем команду ‘ git init ‘
5) выполняем команду ‘ git add . ‘
6) выполняем команду ‘ git commit -m ‘message’ ‘
7) выполняем команду ‘ git push https://github.io/<username>/<projectname>.github.io.git master ‘
8) заходим на github.com в репозитории в раздел ‘settings’, находим ‘GitHub Pages’ и ставим “Source” в положение master branch
9) после этого сайт доступен по адресу <username>.github.io/<projectname>.github.io/public/
 
