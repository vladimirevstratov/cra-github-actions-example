# Начало работы с примером Github Actions

Это пустой проект [Create React App](https://create-react-app.dev/). Я в него добавил файлы для Github Actions, пару библиотек и еще несколько скриптов.
Вы можете склонировать проект себе и адаптировать workflows под свои задачи. Например, вы можете добавить еще файлы workflow для работы с ветками ```develop``` и ```feature```. 

Можете использовать также [каталог экшнов](https://github.com/marketplace?type=actions) от комьюнити. 

# Содержание проекта
### Файлы для работы с Github Actions
Файлы workflow расположены в папке ```./github/workflows```

- ```prod.main.yml``` - основной workflow. Срабатывает на пуш в main ветку.
- ```test.yml``` - пример переиспользуемого workflow, который вызывается из основного в последнем джобе.

### Cкрипты, использующиеся в CI

- ```npm run lint:check``` - проверка стиля кода с помощью Eslint
- ```npm run pretty:check``` - проверка форматирования кода с помощью Prettier
- ```npm run types``` - проверка компиляции Typescript
- ```npm run test``` - выполнение Unit тестов

### Скрипты, использующиеся в CD

- ```npm run build```

# Примечания

В бесплатной версии Github Actions поддерживает 2000 минут и 500 mb хранилища, поэтому имейте это в виду.
