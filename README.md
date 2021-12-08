# Стили кода. Урок 35

# 1. Переменные
- Для именования переменных используйте существительные на английском языке(не транслит!). Имя переменной должно быть осмысленным. Имя может состоять из букв, цифр, символов $ и _, не должно начинаться с цифры.
#### Плохой пример 😠
    var ovoschi;
    var rrfgov;
#### Хороший пример 😃
    var vegetables;
    var car;
    var animals;
# 2. Объекты
__2.1  Создание объекта__
- Для создания объекта используйте фигурные скобки. Не создавайте объекты через конструктор `new Object`.
#### Плохо
    var item = new Object();
#### Хорошо
    var item = {};
__2.2 Зарезервированные и ключевые слова
- Не используйте зарезервированные слова в качестве ключей объектов.
- Не используйте ключевые слова (в том числе измененные). Вместо них используйте синонимы.
#### Плохой пример 😠
   var superman = {
   default: { clark: 'kent' },
   private: true
   };
   
   var superman = {
   class: 'alien'
   };
#### Хороший пример 😃
    var vegetables;
    var car;
    var animals;
