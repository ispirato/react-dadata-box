# React Dadata
React компонент для подсказок с помощью сервиса DaData.ru

Поддерживаются подсказки адресов, организаций, банков.

### Установка
```
npm install react-dadata-box
```
или
```
yarn react-dadata-box
```

### Пример
```javascript
import ReactDadataBox from 'react-dadata-box';

// ...

<ReactDadataBox token="API_KEY" query="Москва" />
```

### Свойства

| Свойство  | Обязательный | Тип | Описание |
| ------------- | ------------- | ------------- | ------------- |
| token  | Да  | string  | Авторизационный токен DaData.ru  |
| type | Да | string | Тип данных, которые необходимо запросить с dadata.ru. Адрес(address), организация(company) или банк(bank)
| placeholder  | Нет  | string  | Текст placeholder  |
| query  | Нет  | string  | Начальное значение поля ввода  |
| autoload  | Нет  | boolean  | Если `true`, то запрос на получение подсказок будет инициирован в фоне сразу, после монтирования компонента  |
| onChange  | Нет  | function(suggestion: ReactDadata.DadataSuggestion)  | Функция, вызываемая при выборе подсказки  |
| autocomplete  | Нет  |string  | параметр описывающий автозаполнение поля, например street-address, если не задан, будет установлен как off  |
| count | Нет | string | Кол-во возвращаемых записей, по умолчанию 10

