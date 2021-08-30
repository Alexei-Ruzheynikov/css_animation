# css_animation

Библиотека анимации AOS
https://michalsnik.github.io/aos/
Подключение библиотеки: aos.js, aos.css. Далее инициализация в js скрипте - AOS.init(); Использование: в тэге html добавляем атрибут data-aos="fade-up" и тд

Поиск подобных библиотек: library css animation.

Указываем в css стиле элемента:
animation-name: moveRight; - название анимации
animation-duration: 1s; - время выполнения анимации
При этом после завершения анимации - вернется в исходное положение
animation-iteration-count: 2; - анимация сработает 2 раза (infinite - бесконечная анимация)
animation-delay: 5s; - анимация начнется через 5 сек (задержка анимации)
animation-direction: reverse; - анимация проигрывается наоборот с конечного кадра в начальный
animation-fill-mode: forwards; - элемент остается в конечной точке по окончанию анимации
animation-timing-function: ease; - скорость воспроизведения анимации - начинается медленно, ускоряется, замедляется к концу (ease-out - начинается быстро, замедляется к концу; linear - с одинаковой скоростью)

Объединенная последовательность:
animation: name duration timing-function delay iteration-count direction fill-mode;(не уверен в правильности, проверить)

Стандартная @keyframes в стилях (moveRight - название анимации)
@keyframes moveRight {
from {
transform: translateX(0);
}
50% {
transform: translate(200px);
}
to {
transform: translateX(100px);
}
}
