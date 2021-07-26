# git-book

## Вступ. Intro.

Минув майже рік з часу, як анонсував свій курс про Git "Fifteen minute git".
Увесь цей час обдумував над аналогією з матеріального світу,
яка би вдало описувала роботу системи контролю версій.
Також хотів би у курсі показати, що Git може стати у пригоді не лише програмістам,
але й авторам статей, книг, музики, векторної графіки і навіть при 
написанні дошок оголошень в інтернеті чи елементарних сайтів-візиток.
Причому все це можуть робити особи без жодного знання програмування.

Almost a year passed since I announced my Git course "Fifteen minute git".
During this time I searched for an analogy from the reality,
which can suitably describe a version control system.
Also, I would like to show in the course, that Git can be useful not only for
programming, but also for articles, books, music, vector graphic and even
for Info walls and landing webpages.
Moreover, all these can be done by people without any programming insight.

Саме таким чином пропоную писати неанглійські дописи на дотичні до IT теми. 
Тобто абзац рідною, абзац англійською. Чому? Та тому, що саме англійська 
термінологія є стандартною в цій галузі.

Exactly this way I propose to write non-english texts about IT.
I.e. A paragraph in native language, followed by an English paragraph.
Why? It is because only English terminology is a standard in the field.

Якщо Ви помічатимите помилки у моїй писанині будь-якою мовою, то сміливо 
виправляйте мене коментарями у репозиторії https://github.com/fifteen-minute-git/git-book ,
де оприлюднюватиму останню версію своїх нотатків.

If you find any mistake in my writings in any language, then
feel free to comment them on the https://github.com/fifteen-minute-git/git-book
repository, where I will publish the latest version of my notes.

Отож до справи! Пропоную до перегляду найперший "нульовий" урок 
свого курсу https://youtu.be/18nW9bo7pFk 
Приємного перегляду! Коментуйте, критикуйте, не соромтеся...

So let's start! I propose you to watch the very first "zero" lesson of
my course https://youtu.be/18nW9bo7pFk
Enjoy watching! Please comment, criticise, don't hesitate...

## Заняття 0. Git як будиночок зі скляних малюночків, що кладуться один на оден (Lesson 0. Git as a building made of glass pictures put one on another)
Нарешті... Ось минув майже рік роздумів. 
Але врешті-решт таки придумав як саме організувати курс про систему контролю версій git.

Finally...Almost year passed in thinking, but finally I found how to organize my git version control course. 

Відео записуватиму рідною українською мовою, але перекладатиму на англійську, якщо про це попросять бодай два англомовні глядачі.

I'll record my videos in my native Ukrainian language, but I'll translate them on request from at least two English-speaking subscribers.

Перш за все хочу сказати, що git можна використовувати не лише для програмування.
Ним з успіхом можуть користуватися непрограмісти. Наприклад при написанні і редагуванні книг, статей, документації і навіть музики (ноти можна записувати у вигляді латинських літер) та векторної графіки.

First of all, let me state that git can be useful not only for programming.
It can be successfully used by non-programmers. For example, it can be used while writing and editing books, articles, documentation and even music (notes can be represented with Latin letters) and vector drawings.

Git подібний на будиночок зі скляних прямокутничків, які кладуть один на оден.
Беремо перший скляний прямокутничок і малюємо на ньому частинку свого малюнку.
Ми знаємо, що фломастер зі скла легко стрирається, тому сміливо творимо. 
Ми можемо експериментувати з кольорами, ми можемо добавляти або стирати лінії, аж поки не будемо задоволені тим, що зробили.
От коли ми більш-менш задоволені результатом наших творчих пошуків, то кладемо зверху на наш скляний прямокутничок з малюночком 
новий скляний прямокутничок і цим ми фіксуємо нашу роботу, оберігаємо її від мимовільної втрати. 
Саме це й називається нашим найпершим (initial) commit.

Git is like a building made of glass rectangles, put one on another.
We take the first glass rectangle and draw a part of our picture on it.
We know that a marker drawing can be easily removed out of glass, so we are brave to art.
We can experiment with colors, we can add or remove lines, until being satisfied with the outcome.
Once we are more or less satisfied with the result of our artistic research, then we put a new glass rectangle onto our
first picture and this way we persist our work, we save it from undesired loss.
Let's call this very fixed picture `initial commit`.

Далі ми продовжуємо малювати нові й нові частини малюнка на нових прямокутничках, крізь які видно наш перший малюнок і всю історію наскрізь.
Малюнки доповнюють одне одного створюючи єдину картину. 
Якщо якась частина нам не сподобалося у результуючому малюнку, то ми можемо її замалювати білою фарбою на наступних прямокутниках.

Then we continue drawing new and new parts of the picture on new rectangles, through which you can see our first picture 
and all the history transparently.
The pictures supplement each other creating a united drawing. 
If we don't like some part in the resulting drawing, then we can clean it using white marker on our next rectangles.

У наступних уроках ми з Вами познайомимся з нашим навчальним репозиторієм. 
Він схожий на ресурс "Інтерактивна карта УГКЦ (Української греко-католицької церкви)" https://map.ugcc.ua/, розроблений УГКЦ для ведення інформації про місцезнаходження парафій та
інформації про них, зокрема розкладів Богослужінь. 

In our next lessons we will get known to our study repository.
It is similar to the "Interactive map of UGCC (Ukrainian Greek-Catholic Church)" https://map.ugcc.ua/. It is developed by UGCC for tracking info about church locations and their descriptions, in particular, timetables of their holy Masses.

Наш навчальний проект буде називатися "Timetable map" і він вміщуватиме інформацію про розташування 
об'єктів і розклад подій, що там відбуваються. На відміну від https://map.ugcc.ua/, наш ресурс
має відкритий код і будь-хто може його модифікувати за допомогою pull-request.

Our educational project is named "Timetable map" and it will contain info about object locations and event timetables taking place there.
In contrast to the https://map.ugcc.ua/, our resource is open source and anyone can modify it using a pull-request.

Про те, що таке "pull request" і про те, що вдосконалювати наш репозиторій зможе навіть особа без
жодного знання програмування зі звичайного браузера йтиметься у наступних уроках.

In our next lessons we will explain the "pull request" term and the thing that anyone can improve our repository even
without any knowledge of programming using regular browser.
