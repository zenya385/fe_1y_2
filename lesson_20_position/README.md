# Урок 20. ПОЗИЦІОНУВАННЯ.

<!--  -->
<!--*  -->
<!--!  -->
<!--?  -->
<!--todo  -->

<!-- ! ====== Властивість position ====== -->

position: static | relative | absolute | fixed | sticky

Властивість position дає нам змогу точно задати нове місце положення блоку відносно того місця, де він знаходився в нормальному потоці документа.

<!-- todo == position: static == -->

За замовчуванням встановлено значення static.

<!-- todo == position: relative (Відносне позиціонування) == -->

Під час використання відносного позиціонування елемент залишається в потоці сторінки, тобто сусідні елементи не займають його місце.
--Властивості top, left, bottom і right дозволяють вказати зміщення елемента (візуальне) щодо його вихідного положення. Можуть приймати від'ємні значення.

<!-- todo == position: absolute (Абсолютне позиціонування)== -->

Під час використання абсолютного позиціонування елемент виривається з потоку сторінки, тобто сусідні елементи займають його місце. Відлік значень top, left, bottom і right для абсолютно позиційованого елемента ведеться щодо найближчого предка з позиціонуванням, відмінного від статичного. Якщо такого предка не буде, то відлік буде здійснюватися від меж елемента <body>.

Якщо не поставити батьківському блоку відносне позиціонування, то всі три p.label опиняться у верхньому правому куті вікна, оскільки значення top і right будуть відраховуватися щодо елемента <body>.

<!-- todo == position: fixed (Фіксоване позиціонування)== -->

У разі фіксованого позиціонування, елемент вилучається з потоку сторінки і позиціонується щодо в'юпорту (вікна браузера). Це створює ефект фіксації елемента в певному місці екрану при прокручуванні сторінки.
Фіксоване позиціонування використовується для закріплених хедерів з навігацією, спливаючих вікон, чатів з менеджером на сторінках інтернет-магазинів тощо.

example: https://codepen.io/goit-academy/pen/OJMevjB

<!-- todo == position: sticky (Липке позиціонування) == -->

Липке позиціонування (sticky) - це ніби комбінація властивостей relative і fixed. Для початку подивіться на ілюстрацію, на якій липке позиціонування задається елементам з літерами A і B, таким чином відразу буде зрозуміло.

Для реалізації липкого позиціонування необхідні всього три умови:

1. У липкого елемента повинно бути встановлено позиціонування position: sticky.
2. У липкого елемента повинно бути встановлено положення, наприклад top: 0.
3. Елемент-контейнер повинен бути більшим по висоті за липкий елемент.

example: https://codepen.io/goit-academy/pen/pogXLWz

 <!--! ====== Властивість z-index ====== -->

z-index: <числове значеннч>;

exemple: https://www.edu.goit.global/uk/learn/266288/30288/30293/textbook

<!--! ====== Властивість overflow ====== -->

overflow: visible | hidden | scroll | auto

Розміри елемента визначаються контентом всередині нього або задаються явно. Що відбувається у разі зміни контенту всередині елемента? Наприклад, якщо не встановити висоту, то вона буде збільшуватися, доки в елементі не поміститься увесь контент.

-visible - видимий переповнюючий вміст. Значення за замовчуванням.
-hidden - все, що виходить за межі блоку, буде візуально приховане.
-scroll - у разі переповнення з'являються горизонтальна і вертикальна смуги прокручування, навіть якщо потрібна тільки одна.
-auto - схоже на значення scroll, але смуги прокручування показуються тільки там, де вони дійсно необхідні, а не всі відразу.

<!-- todo == overflow: visible (видимий переповнюючий вміст. Значення за замовчуванням.) == -->

exemple:

<!-- todo == overflow: hidden (все, що виходить за межі блоку, буде візуально приховане.) == -->

exemple:

<!-- todo == overflow: scroll (у разі переповнення з'являються горизонтальна і вертикальна смуги прокручування, навіть якщо потрібна тільки одна.) == -->

exemple:

<!-- todo == overflow: auto (схоже на значення scroll, але смуги прокручування показуються тільки там, де вони дійсно необхідні, а не всі відразу.) == -->

exemple: