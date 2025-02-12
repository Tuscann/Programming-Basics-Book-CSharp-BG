# Глава 5. Повторения (цикли)

В настоящата глава ще се запознаем с конструкциите за **повторение на група команди**, известни в програмирането с понятието "**цикли**". Ще напишем няколко цикъла с използване на оператора **`for`** в най-простата му форма. Накрая ще решим няколко практически задачи, изискващи повторение на поредица от действия, като използваме цикли.

## Видео

<div class="video-player">
  Гледайте видео-урок по тази глава тук: <a target="_blank"
  href="https://www.youtube.com/watch?v=Xjwjk9yS4uw">
  https://www.youtube.com/watch?v=Xjwjk9yS4uw</a>.
</div>
<script src="/assets/js/video.js"></script>

## Повторения на блокове код (**for цикъл**)

В програмирането често пъти се налага **да изпълним блок с команди няколко пъти**. За целта се използват т.нар. **цикли**. Нека разгледаме един пример за **`for` цикъл**: 

![](assets/chapter-5-images/00.For-loop-01.png)

Цикълът започва с **оператора `for`** и преминава през всички стойности за дадена променлива в даден интервал, например всички числа от 1 до 10 включително, и за всяка стойност изпълнява поредица от команди.

В декларацията на цикъла може да се зададе **начална стойност** и **крайна стойност**. **Тялото на цикъла** обикновено се огражда с къдрави скоби **`{ }`** и представлява блок с една или няколко команди. На фигурата по-долу е показана структурата на един **`for` цикъл**:

![](assets/chapter-5-images/00.For-loop-02.png)

В повечето случаи един **`for` цикъл** се завърта от **`1`** до **`n`** пъти (например от 1 до 10). Целта на цикъла е да се премине последователно през числата 1, 2, 3, ..., n и за всяко от тях да се изпълни някакво действие. В примера по-горе променливата **`i`** приема стойности от 1 до 10 и в тялото на цикъла сe отпечатва текущата стойност. Цикълът се повтаря 10 пъти и всяко от тези повторения се нарича "**итерация**".

### Пример: Числа от 1 до 100

Да се напише програма, която **печата числата от 1 до 100**. Програмата не приема вход и отпечатва числата от 1 до 100 едно след друго, по едно на ред.

#### Насоки и подсказки

Можем да решим задачата с **`for` цикъл** , с който преминаваме с променливата **`i`** през числата от 1 до 100 и ги печатаме:

![](assets/chapter-5-images/01.Numbers-1-to-100-01.png)

**Стартираме** програмата с [**Ctrl+F5**] и я **тестваме**:

![](assets/chapter-5-images/01.Numbers-1-to-100-02.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#0](https://judge.softuni.bg/Contests/Practice/Index/510#0)

Трябва да получите **100 точки** (напълно коректно решение).

## Code Snippet за for цикъл във Visual Studio

Докато програмираме, постоянно се налага да пишем цикли, десетки пъти всеки ден. Затова в повечето среди за разработка (IDE) има **шаблони за код** (**code snippets**) за писане на цикли. Един такъв шаблон е **шаблонът за `for` цикъл във Visual Studio**. Напишете **`for`** в редактора за C# код във Visual Studio и **натиснете два пъти** [**Tab**]. Visual Studio ще разгъне за вас шаблон и ще напише цялостен **`for` цикъл**:

![](assets/chapter-5-images/00.For-loop-code-snippet.png)

**Опитайте сами**, за да усвоите умението да ползвате шаблона за код за **`for` цикъл** във Visual Studio.

### Пример: Числа до 1000, завършващи на 7

Да се напише програма, която намира всички числа в интервала [**1…1000**], които завършват на 7. 

#### Насоки и подсказки

Задачата можем да решим като комбинираме **`for` цикъл** за преминаваме през числата от 1 до 1000 и **проверка** за всяко число дали завършва на 7. Има и други решения, разбира се, но нека решим задачата чрез **завъртане на цикъл + проверка**:

![](assets/chapter-5-images/02.Numbers-ending-in-7-01.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#1](https://judge.softuni.bg/Contests/Practice/Index/510#1)

### Пример: Всички латински букви

Да се напише програма, която отпечатва буквите от латинската азбука: **a, b, c, …, z**.

#### Насоки и подсказки

Тук трябва да се отбележи, че **`for` циклите** не работят само с числа. Може да решим задачата като завъртим **`for` цикъл**, който преминава последователно през всички букви от латинската азбука:

![](assets/chapter-5-images/03.Latin-letters-01.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#2](https://judge.softuni.bg/Contests/Practice/Index/510#2)

### Пример: Сумиране на числа

Да се напише програма, която **въвежда `n` цели числа и ги сумира**.

* От първия ред на входа се въвежда броят числа **`n`**.
* От следващите **`n`** реда се въвежда по едно число.
* Числата се сумират и накрая се отпечатва резултатът.

#### Примерен вход и изход

| Вход | Изход |
| --- | --- |
| 2<br>10<br>20 | 30 |
| 3<br>-10<br>-20<br>-30 | -60 |
| 4<br>45<br>-20<br>7<br>11<br> | 43 |
| 1<br>999 | 999 | 
| 0 | 0 |

#### Насоки и подсказки

Можем да решим задачата за сумиране на числа по следния начин:
 - Четем входното число **`n`**.
 - Започваме първоначално със сума **`sum = 0`**.
 - Въртим цикъл от 1 до **`n`**. На всяка стъпка от цикъла четем число **`num`** и го добавяме към сумата **`sum`**.
 - Накрая отпечатваме получената сума **`sum`**.
 
Ето и сорс кодa на решението:

![](assets/chapter-5-images/04.Sum-numbers-01.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#3](https://judge.softuni.bg/Contests/Practice/Index/510#3)

### Пример: Най-голямо число

Да се напише програма, която въвежда **n цели числа** (**n** > 0) и намира **най-голямото** измежду тях. На първия ред на входа се въвежда броят числа **n**. След това се въвеждат самите числа, по едно на ред. Примери:

#### Примерен вход и изход

| Вход | Изход |
| --- | --- |
| 2<br>100<br>99 | 100 | 
| 3<br>-10<br>20<br>-30 | 20 |
| 4<br>45<br>-20<br>7<br>99<br> | 99 | 
| 1<br>999 | 999 |
| 2<br>-1<br>-2 | -1 |

#### Насоки и подсказки

Първо въвеждаме едно число **`n`** (броят числа, които предстои да бъдат въведени). Задаваме на текущия максимум **`max`** първоначална неутрална стойност, например **-10000000000000** (или **`int.MinValue`**). С помощта на **`for` цикъл**, чрез който итерираме **n-1 пъти**, прочитаме по едно цяло число **`num`**. Ако прочетеното число **`num`** е по-голямо от текущия максимум **`max`**, присвояваме стойността на **`num`** в променливата **`max`**. Накрая, в **`max`** трябва да се е запазило най-голямото число. Отпечатваме го на конзолата.

![](assets/chapter-5-images/05.Max-number-01.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#4](https://judge.softuni.bg/Contests/Practice/Index/510#4)

### Пример: Най-малко число

Да се напише програма, която въвежда **n цели числа** (**n** > 0) и намира **най-малкото** измежду тях. Първо се въвежда броя числа **n**, след тях още **n** числа по едно на ред. 

#### Примерен вход и изход

| Вход | Изход | 
| --- | --- |
| 2<br>100<br>99 | 99 |
| 3<br>-10<br>20<br>-30 | -30 |
| 4<br>45<br>-20<br>7<br>99<br> | -20 |

#### Насоки и подсказки

Задачата е абсолютно аналогична с предходната:

![](assets/chapter-5-images/06.Min-number-01.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#5](https://judge.softuni.bg/Contests/Practice/Index/510#5)


### Пример: Лява и дясна сума

Да се напише програма, която въвежда **2 \* n цели числа** и проверява дали **сумата на първите n числа** (лява сума) е равна на **сумата на вторите n числа** (дясна сума). При равенство се печата **"Yes" + сумата**, иначе се печата **"No" + разликата**. Разликата се изчислява като положително число (по абсолютна стойност). 

#### Примерен вход и изход

| Вход | Изход | Вход | Изход |
| --- | --- | --- | --- | 
| 2<br>10<br>90<br>60<br>40 | Yes, sum = 100 | 2<br>90<br>9<br>50<br>50 | No, diff = 1 |

#### Насоки и подсказки

Първо въвеждаме числото **n**, след това първите **n** числа (**лявата** половина) и ги сумираме. Продължаваме с въвеждането на още **n** числа (**дясната** половина) и намираме и тяхната сума. Изчисляваме **разликата** между намерените суми по абсолютна стойност: **`Math.Abs(leftSum - rightSum)`**. Ако разликата е **0**, отпечатваме **"Yes" + сумата**, в противен случай - отпечатваме **"No" + разликата**.

![](assets/chapter-5-images/07.Left-and-right-sum-01.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#6](https://judge.softuni.bg/Contests/Practice/Index/510#6)


### Пример: Четна / нечетна сума

Да се напише програма, която въвежда **n цели числа** и проверява дали **сумата на числата на четни позиции** е равна на **сумата на числата на нечетни позиции**. При равенство печата **"Yes" + сумата**, иначе печата **"No" + разликата**. Разликата се изчислява по абсолютна стойност. 

#### Примерен вход и изход

| Вход | Изход |
| --- | --- |
| 4<br>10<br>50<br>60<br>20 | Yes<br>Sum = 70 |
| 4<br>3<br>5<br>1<br>-2 | No<br>Diff = 1 |
| 3<br>5<br>8<br>1 | No<br>Diff = 2 |

#### Насоки и подсказки

Въвеждаме числата едно по едно и изчисляваме двете **суми** (на числата на **четни** позиции и на числата на **нечетни** позиции). Както в предходната задача, изчисляваме абсолютната стойност на разликата и отпечатваме резултата (**"Yes" + сумата** при разлика 0 или **"No" + разликата** в противен случай).

![](assets/chapter-5-images/08.Odd-even-sum-01.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#7](https://judge.softuni.bg/Contests/Practice/Index/510#7)

### Пример: Сумиране на гласните букви

Да се напише програма, която въвежда **текст** (стринг), изчислява и отпечатва **сумата от стойностите на гласните букви** според таблицата по-долу:

| a | e | i | o | u | 
| :---: | :---: | :---: | :---: | :---: |
| 1 | 2 | 3 | 4 | 5 |

#### Примерен вход и изход

| Вход | Изход | Вход | Изход | 
| --- | --- | --- | --- |
| hello | 6<br>(e+o = 2+4 = 6) | bamboo | 9<br>(a+o+o = 1+4+4 = 9) |
| hi | 3<br>(i = 3) | beer | 4<br>(e+e = 2+2 = 4) |

#### Насоки и подсказки

Прочитаме входния текст **`s`**, нулираме сумата и завъртаме цикъл от **0** до **`s.Length-1`** (дължината на текста -1). Проверяваме всяка буква **`s[i]`** дали е гласна и съответно добавяме към сумата стойността ѝ.

![](assets/chapter-5-images/09.Vowels-sum-01.png)

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#8](https://judge.softuni.bg/Contests/Practice/Index/510#8)

## Какво научихме от тази глава?

Можем да повтаряме блок код с **`for` цикъл**:

![](assets/chapter-5-images/00.For-loop-01.png)

Можем да четем поредица от **`n`** числа от конзолата:

![](assets/chapter-5-images/00.For-loop-03.png)

## Упражнения: повторения (цикли)

### Празно Visual Studio решение (Blank Solution)

Създаваме празно решение **(Blank Solution)** във Visual Studio, за да организираме по-добре задачите за упражнение. Целта на този **blank solution** e да съдържа **по един проект за всяка задача** от упражненията.
  
![](assets/chapter-5-images/00.Blank-visual-studio.png)

Задаваме **да се стартира по подразбиране текущият проект** (не първият в решението). Кликваме с десен бутон на мишката върху **Solution 'Loops'** -> [**Set StartUp Projects…**] -> [**Current selection**].

### Задача: Елемент, равен на сумата на останалите

Да се напише програма, която въвежда **n цели числа** и проверява дали сред тях съществува число, което е равно на сумата на всички останали. Ако има такъв елемент, се отпечатва **"Yes" + неговата стойност**, в противен случай - **"No" + разликата между най-големия елемент и сумата на останалите** (по абсолютна стойност). 

#### Примерен вход и изход

| Вход | Изход | Коментар |
| --- | --- | :---: |
| 7<br>3<br>4<br>1<br>1<br>2<br>12<br>1 | Yes<br>Sum = 12 | 3 + 4 + 1 + 2 + 1 + 1 = 12 |
| 4<br>6<br>1<br>2<br>3 | Yes<br>Sum = 6 | 1 + 2 + 3 = 6 |
| 3<br>1<br>1<br>10 | No<br>Diff = 8 | &#124;10 - (1 + 1)&#124; = 8 |
| 3<br>5<br>5<br>1 | No<br>Diff = 1 | &#124;5 - (5 + 1)&#124; = 1 |
| 3<br>1<br>1<br>1 | No<br>Diff = 1 | - |

#### Насоки и подсказки

Трябва да изчислим **сумата** на всички елементи, да намерим **най-големия** от тях и да проверим търсеното условие.

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#9](https://judge.softuni.bg/Contests/Practice/Index/510#9)

### Задача: Четни / нечетни позиции

Напишете програма, която чете **n числа** и пресмята **сумата**, **минимума** и **максимума** на числата на **четни** и **нечетни** позиции (броим от 1). Когато няма минимален / максимален елемент, отпечатайте **"No"**. 

#### Примерен вход и изход

| Вход | Изход | Вход | Изход |
| --- | --- | --- | --- |
| 6<br>2<br>3<br>5<br>4<br>2<br>1 | OddSum=9,<br>OddMin=2,<br>OddMax=5,<br>EvenSum=8,<br>EvenMin=1,<br>EvenMax=4 | 2<br>1.5<br>-2.5 | OddSum=1.5,<br>OddMin=1.5,<br>OddMax=1.5,<br>EvenSum=-2.5,<br>EvenMin=-2.5,<br>EvenMax=-2.5 |
| 1<br>1 | OddSum=1,<br>OddMin=1,<br>OddMax=1,<br>EvenSum=0,<br>EvenMin=No,<br>EvenMax=No | 0 | OddSum=0,<br>OddMin=No,<br>OddMax=No,<br>EvenSum=0,<br>EvenMin=No,<br>EvenMax=No |
| 5<br>3<br>-2<br>8<br>11<br>-3 | OddSum=8,<br>OddMin=-3,<br>OddMax=8,<br>EvenSum=9,<br>EvenMin=-2,<br>EvenMax=11 | 4<br>1.5<br>1.75<br>1.5<br>1.75 | OddSum=3,<br>OddMin=1.5,<br>OddMax=1.5,<br>EvenSum=3.5,<br>EvenMin=1.75,<br>EvenMax=1.75 |
| 1<br>-5 | OddSum=-5,<br>OddMin=-5,<br>OddMax=-5,<br>EvenSum=0,<br>EvenMin=No,<br>EvenMax=No | 3<br>-1<br>-2<br>-3 | OddSum=-4,<br>OddMin=-3,<br>OddMax=-1,<br>EvenSum=-2,<br>EvenMin=-2,<br>EvenMax=-2 |

#### Насоки и подсказки

Задачата обединява няколко предходни задачи: намиране на **минимум**, **максимум** и **сума**, както и обработка на елементите от **четни и нечетни позиции**. Припомнете си ги.

В тази задача е по-добре да се работи с **дробни числа** (не цели). Сумата, минимумът и максимумът също са дробни числа. Трябва да използваме **неутрална начална стойност** при намиране на минимум / максимум, например **1000000000.0** и **-1000000000.0**. Ако получим накрая неутралната стойност, печатаме **“No”**.

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#10](https://judge.softuni.bg/Contests/Practice/Index/510#10)


### Задача: Еднакви двойки

Дадени са **2 \* n числа**. Първото и второто формират **двойка**, третото и четвъртото също и т.н. Всяка двойка има **стойност** – сумата от съставящите я числа. Напишете програма, която проверява **дали всички двойки имат еднаква стойност**. В случай, че е еднаква отпечатайте **"Yes, value=…" + стойността**, в противен случай отпечатайте **максималната разлика** между две последователни двойки в следния формат - **"No, maxdiff=…" + максималната разлика**. 

#### Примерен вход и изход

| Вход | Изход | Коментар |
| --- | --- | :---: | 
| 3<br>1<br>2<br>0<br>3<br>4<br>-1| Yes, value=3 | стойности = {3, 3, 3}<br>еднакви стойности | 
| 2<br>1<br>2<br>2<br>2 | No, maxdiff=1 | стойности = {3, 4}<br>разлики = {1}<br>макс. разлика = 1 |
| 4<br>1<br>1<br>3<br>1<br>2<br>2<br>0<br>0 | No, maxdiff=4 | стойности = {2, 4, 4, 0}<br>разлики = {2, 0, 4}<br>макс. разлика = 4 |
| 1<br>5<br>5 | Yes, value=10 | стойности = {10}<br>една стойност<br>еднакви стойности |
| 2<br>-1<br>0<br>0<br>-1 | Yes, value=-1 | стойности = {-1, -1}<br>еднакви стойности | 
| 2<br>-1<br>2<br>0<br>-1 | No, maxdiff=2 | стойности = {1, -1}<br>разлики = {2}<br>макс. разлика = 2 |

#### Насоки и подсказки

Прочитаме входните числа **по двойки**. За всяка двойка пресмятаме **сумата** ѝ. Докато четем входните двойки, за всяка двойка, без първата, трябва да пресметнем **разликата с предходната**. За целта е необходимо да пазим в отделна променлива сумата на предходната двойка. Накрая намираме **най-голямата разлика** между две двойки. Ако е **0**, печатаме **“Yes”** + стойността, в противен случай - **“No”** + разликата

#### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/510#11](https://judge.softuni.bg/Contests/Practice/Index/510#11)


## Упражнения: графични и уеб приложения

### Задача: Чертане с костенурка – графично GUI приложение

Целта на следващото упражнение е да си поиграем с една **библиотека за рисуване**, известна като **“графика с костенурка” (turtle graphics)**. Ще изградим графично приложение, в което ще **рисуваме различни фигури**, придвижвайки нашата **“костенурка”** по екрана чрез операции от типа “отиди напред 100 позиции”, “завърти се надясно на 30 градуса”, “отиди напред още 50 позиции”. Приложението ще изглежда приблизително така:

![code](assets/chapter-5-images/13.Turtle-graphics-01.png)

Нека първо се запознаем с **концепцията за рисуване “Turtle Graphics”**. Може да разгледаме следните източници:

* дефиниция на понятието “turtle graphics”: [http://c2.com/cgi/wiki?TurtleGraphics](http://c2.com/cgi/wiki?TurtleGraphics)
* статия за “turtle graphics” в Wikipedia – [https://en.wikipedia.org/wiki/Turtle_graphics](https://en.wikipedia.org/wiki/Turtle_graphics)
* интерактивен онлайн инструмент за чертаене с костенурка – [https://blockly-games.appspot.com/turtle](https://blockly-games.appspot.com/turtle)

Започваме, като създаваме нов **C# Windows Forms проект**:

![](assets/chapter-5-images/13.Turtle-graphics-02.png)

Инсталираме **NuGet** пакета **"Nakov.TurtleGraphics"** към нашия нов Windows Forms проект. От Visual Studio може да се добавят **външни библиотеки** (пакети) към съществуващ C# проект. Те добавят допълнителна функционалност към нашите приложения. Официалното хранилище (repository) за C# библиотеки се поддържа от Microsoft и се нарича **NuGet** ([http://www.nuget.org/](http://www.nuget.org/)).

Кликаме с десен бутон на мишката върху проекта в **Solution Explorer** и избираме [**Manage NuGet Packages…**]:
 
![](assets/chapter-5-images/13.Turtle-graphics-03.png)

Ще се отвори прозорец за търсене и инсталиране на **NuGet** пакети. Нека потърсим пакети по ключова дума **“nakov”**. Ще излязат няколко пакета. От тях избираме пакет **“Nakov.TurtleGraphics”**. Натискаме [**Install**], за да го инсталираме към нашия C# проект:
 
![](assets/chapter-5-images/13.Turtle-graphics-04.png)

Към нашия C# проект вече е включена външната библиотека **“Nakov.TurtleGraphics”**. Тя дефинира клас **Turtle**, който представлява **костенурка за рисуване**. За да го използваме, трябва да добавим в C# кода за нашата форма (**Form1.cs**). Добавяме следния код, най-отгоре в началото на файла:
  
![](assets/chapter-5-images/13.Turtle-graphics-05.png)

Сега трябва да сложим **три бутона** във формата и да променим **имената** и **свойствата** им, както е посочено по-долу:
 
![](assets/chapter-5-images/13.Turtle-graphics-06.png)

Кликваме два пъти върху бутона [**Draw**], за да въведем кода, който да се изпълни при натискането му. Пишем следния код:

![](assets/chapter-5-images/13.Turtle-graphics-07.png)

Този код мести и върти костенурката, която в началото е в центъра на екрана (в средата на формата), и чертае равностранен триъгълник. Може да го редактирате и да си поиграете с него.

**Стартираме** приложението с [**Ctrl+F5**]. Тестваме го дали работи (натискаме [**Draw**] бутона няколко пъти):

![](assets/chapter-5-images/13.Turtle-graphics-08.png)

Сега може да променим и усложним кода на **костенурката**: 

![](assets/chapter-5-images/13.Turtle-graphics-09.png)

Отново **стартираме** приложението с [**Ctrl+F5**]. Тестваме дали работи новата програма за костенурката:

![](assets/chapter-5-images/13.Turtle-graphics-10.png)

Вече нашата костенурката чертае по-сложни фигури чрез приятно анимирано движение.

Нека напишем кода и за останалите два бутона. Целта на бутона [**Reset**] е да изтрие графиката и да започне да чертае на чисто:

![](assets/chapter-5-images/13.Turtle-graphics-11.png)

Целта на бутона [**Show / Hide Turtle**] е да показва или скрива костенурката: 

![](assets/chapter-5-images/13.Turtle-graphics-12.png)

Отново **стартираме** приложението с [**Ctrl+F5**] и го тестваме, дали работи коректно.

### Задача: * Чертане на шестоъгълник с костенурката

Добавете бутон [**Hexagon**], който чертае правилен шестоъгълник:

![](assets/chapter-5-images/13.Turtle-graphics-13.png)

**Подсказка:**

В цикъл повторете 6 пъти следното:
* Ротация на 60 градуса.
* Движение напред 100.

### Задача: * Чертане на звезда с костенурката

Добавете бутон [**Star**], който чертае звезда с 5 върха (**петолъчка**), като на фигурата по-долу:

![](assets/chapter-5-images/13.Turtle-graphics-14.png)

**Подсказка:**

Сменете цвета: **`Turtle.PenColor` = `Color.Green`**. 

В цикъл повторете 5 пъти следното:
* Движение напред 200.
* Ротация на 144 градуса.

### Задача * Чертане на спирала с костенурката

Добавете бутон [**Spiral**], който чертае спирала с 20 върха като на фигурата по-долу:

![](assets/chapter-5-images/13.Turtle-graphics-15.png)

**Подсказка:**

Чертайте в цикъл, като движите напред и завъртате. С всяка стъпка увеличавайте постепенно дължината на движението напред и завъртайте на 60 градуса.

### Задача: * Чертане на слънце с костенурката

Добавете бутон [**Sun**], който чертае слънце с 36 върха като на фигурата по-долу:

![](assets/chapter-5-images/13.Turtle-graphics-16.png)

### Задача: * Чертане на спирален триъгълник с костенурката

Добавете бутон [**Triangle**], който чертае три триъгълника с по 22 върха като на фигурата по-долу:

![](assets/chapter-5-images/13.Turtle-graphics-17.png)

**Подсказка:**

Чертайте в цикъл като движите напред и завъртате. С всяка стъпка увеличавайте с 10 дължината на движението напред и завъртайте на 120 градуса. Повторете 3 пъти за трите триъгълника.
