# Стили кода. Урок 35

# 1. Переменные
- Для именования переменных используйте существительные на английском языке(не транслит!). Имя переменной должно быть осмысленным. Имя может состоять из букв, цифр, символов $ и _, не должно начинаться с цифры.
#### Плохой пример 😠
``` js
    var ovoschi;
    var rrfgov;
```
#### Хороший пример 😃
``` js
    var vegetables;
    var car;
    var animals;
```
# 2. Объекты
__2.1  Создание объекта__
- Для создания объекта используйте фигурные скобки. Не создавайте объекты через конструктор `new Object`.
#### Плохо 😠
``` js
    var item = new Object();
```
#### Хорошо 😃
``` js   
   var item = {};
```
__2.2 Зарезервированные и ключевые слова__
- Не используйте зарезервированные слова в качестве ключей объектов.
- Не используйте ключевые слова (в том числе измененные). Вместо них используйте синонимы.
#### Плохой пример 😃
``` js
   var superman = {
   default: { clark: 'kent' },
   private: true
   };
   
   var superman = {
   class: 'alien'
   };
```
#### Хороший пример 😃
``` js
    var superman = {
    defaults: { clark: 'kent' },
    hidden: true
    };
    
    var superman = {
    type: 'alien'
    };
```
__2.3 Создание обьекта на 3 и более элементов.__
    
При создании обьектов, равно как и массивов, содержащих большое количество свойств(элементов), и тем самым образующих строки, длиной более 20 символов, необходимо выполнять ряд условий:

- Открывающая скобка располагается на той же строке;
- Каждое свойство оформляется на новой строке;
- Пробел после двоеточия;
- Закрывающая скобка располагается на новой строке.
#### Плохой пример 😠
``` js
   var superman = {defaults: { clark: 'kent' }, type: 'alien', hidden: true};
```
#### Хороший пример 😃
``` js
  var superman = {
  defaults: { clark: 'kent' },
  type: 'alien',
  hidden: true
  };
```
# 3.Функции

- Для объявления функции в начале идёт ключевое слово function, после него имя функции, затем список параметров в круглых скобках через запятую.
- Переменные, объявленные внутри функции, видны только внутри этой функции.
- У функции есть доступ к внешним переменным.
- Имя функции должно быть глаголом на английском языке или начинаться с него. Для имён, состоящих из нескольких слов, используйте camelCase.
#### Плохой пример 😠
``` js
    let userName = 'Irina';

    function showMessage(){let userName = "Polina"; // объявляем локальную переменную
    let message = 'Привет, ' + userName;
    alert(message);
    }
// функция создаст и будет использовать свою собственную локальную переменную userName и игнорировать глобальную.
    showMessage();
};
```
#### Хороший пример 😃
``` js
    let userName = 'Irina';

    function showMessage() {
    let message = 'Привет, ' + userName;
    alert(message);
    }

    showMessage()
```
# 4.
