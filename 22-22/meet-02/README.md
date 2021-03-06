# Среща 2 - Въведение в WEB - Семантични тагове и формуляри

#### 💡 - Какво разгледахме днес
- Семантична версия на HTML таговете;
- Списъци
- HTML формуляри.

 #### 📚 - Ресурси и материали
- [Видео от срещата](https://www.youtube.com/watch?v=bwS6TKElSMU&list=PLyZOguednhL5s3LH63o1q8CHhfNk4kvf1&index=3)
- [Решение на домашна работа](./source/homework-solution)
- [Сорс код от срещата](./source/work-in-class-solution)

 #### 🕹️ - Задачи за упражнения
- [Работа в час](./cw/README.md)
- [Домашна работа](./hw/README.md)

### **Семантична версия на HTML тагове**
Както говорихме вече многократно, структурните тагове имат за цел да предоставят на разработчиците ИНФОРМАЦИЯ за ИНФОРМАЦИЯТА която съдържат, но е доста трудно това да се случи само и единствено със скромния набор от елементи с които разполагаме. Основната ни ракета носител се явява тага **DIV** който в целия си блясък, просто създава блок, без да има претенции да прави нещо по специално от това да играе ролята на своеобразен **етикет** за информацията, която съдържа. 
Какво да правим ако искаме да вкараме малко повече логика в напълно безличния таг, отговора е да ползваме семантичните му разновидности. Семантиката е смисъла, който придаваме на нещо. В нашия, случай това се свежда до въпроса къде се ползва въпросния елемент:
- **\<section\>\<\/section\>** - описва блок, който съдържа блокове свързана информация.
- **\<article\>\<\/article\>** - обикновенно е част от **section** описва елемент от въпросната свързана информация
- **\<header\>\<\/header\>** - описва основно съдържание / заглавие в рамките на **article** или **div**
- **\<footer\>\<\/footer\>** - описва второстепенно съдържание съдържание / заглавие в рамките на **article** или **div**

### **Списъци**
Човек е добре да живее идва момента в който трябва да организира списък, под каквато и да е форма:
- за покупки
- за свадби 
- за задачи
- за купони
Даже сега залитнахме в тази посока и описахме списък. В HTML списъците групират съдържание, което е свъразно и се състои от един елемент и неговите атрибути. Списъците се състоят от две части:
- контейнер за списък - дефинира се с тага <ul></ul>
- елементи на списъка - дефинира се с тага <li></li>

```html
<span>Списък за пазара</span>
<ul>
    <li>500 грама Масло</li>
    <li>1 литър мляко</li>
    <li>3 броя яйца</li>
    <li>1 билет за лотарията</li>
</ul>
```

### **HTML формуляри**
Формулярите са единствения механизъм за комуникация с Back-end, логическия механизъм за управление на WEB приложенията. Формите са визуална репрезентация с която потребителя може да изрази своята воля с която да получи или даде информация. 

Всички формуляри се дефинират в елемента **form**. В него се дефинират всички видове форми, които да позволят на потребителя да въведе информация. 

```html
<form></form>
```

Информацията може да се дефинира като:
- свободен текст
- числа
- време
- цветове
- и др.. 

Основния елемент за формуляр се дефинира с тага **input**. Като атрибут на същия се подава предратилено дефинирана стойност, за визуалния компонент, който браузара ще визуализира за да вземе информация от клиента.

```html
<form>
    <!-- Текстово поле -->
    <input type="text"/>

    <!-- Календар -->
    <input type="date"/>
</form>
```

Всеки формуляр, може да дефинира специално название, с помоща на атрибута **name**, който е изключително важен, в контекста обработката му от страна на **сървъра** (но това е тема за друг път).