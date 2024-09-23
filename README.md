# Виды ошибок

## Синтаксические
Синтаксические баги распространены среди новичков. Они относятся к категории «самых безобидных». С данной категорией ошибок способны справиться компиляторы тех или иных языков. Соответствующие инструменты показывают, где допущена неточность. Остается лишь понять, как исправить ее.

Синтаксические ошибки – ошибки синтаксиса, правил языка. Вот пример в Паскале:
<div align="center"> 
  <img src="https://lh6.googleusercontent.com/asWqELvce9_mpHKV9iueSrmjuYEyqo9ZN5jxDUFXMLkWZZUa2BCM_6-br2zI7KVTwju4KYpxQ6AyXei60u03Jb-aQMrfyyhwYZBGvOdU4rOUyu6Qt_oryOKy-7TC59A6_-1AL9fDzdjIvhXaUFzhy-WC14jB61Tb-VtiI9RqKZNlBmABpQaHGmgRia5-b43W6sXUNDe7RA"/> 
</div>
Виды ошибок программного обеспечения. Баги
Код написан неверно. Согласно действующим синтаксическим нормам, в Pascal в первой строчке нужно в конце поставить точку с запятой.

## Логические
Тут стоит выделить обычные и арифметические типы. Вторые возникают, когда программе при работе необходимо вычислить много переменных, но на каком-то этапе расчетов возникают неполадки или нечто непредвиденное. Пример – получение в результатах «бесконечности».

Логические сбои обычного типа – самые сложные и неприятные. Их тяжелее всего обнаружить и исправить. С точки зрения языка программа может быть написана идеально, но работать неправильно. Подобное явление – следствие логической ошибки. Компиляторы их не обнаруживают.

Пример логической ошибки в программе. Тут:
<div align="center"> 
  <img src="https://lh6.googleusercontent.com/ej7U3OO9mutiZ-qEGsnN8QjtvLdsZyQs9WKj9kwJrpoFWMDrXEhlUiqPa8d_3lx6yqUYXx81nkxlJ1BlIQfGx7v2cxPOO3VYrazwDh6pA1MDcVFQ0extaITthcAtZQ1DbBrEaAwUUgVBU83fKQ7RCF2ueW1-Lf45xSKzzJ8R4H8VJvn3nMnStI4lBs0n0-YuZwq4AG33Eg"/> 
</div>
Происходит сравнение значения i с 15.

На экран выводится сообщение, если I = 15.

В заданном цикле i не будет равно 15. Связано это с диапазоном значений – от 1 до 10.

Может показаться, что ошибка безобидная. В приведенном примере так и есть, но в более крупных программах такое явление приводит к серьезным последствиям.

## Время выполнения
Run-time сбои – это ошибка времени выполнения программы. Встречается даже когда исходный код лишен логических и синтаксических ошибок. Связаны такие неполадки с ходом выполнения программного продукта. Пример – в процессе функционирования ПО был удален файл, считываемый программой. Если игнорировать подобные неполадки, можно столкнуться с аварийным завершением работы контента.
<div align="center"> 
  <img src="https://lh5.googleusercontent.com/om_0sqObiqWUNgb-04O7XfyZooPF5vTEqE01hm0YLADuvSlMEMqtqe7p5GY7D_nM9tbjiwPyKsrbxLqbKGsaWvnTZXPWz3i3xX0nqQwwx8ZVcctPcX63n1ayzKztN2gfkjYnqGCqjzlUJVczt0fAJEVuBTSTQ9QFyxyLDsQmxdkyvuX3-ZoAYlzbE2ZU-ZGVGERoT2F8TQ"/> 
</div>
Самый распространенный пример в данной категории – это неожиданное деление на ноль. Предложенный фрагмент кода с точки зрения синтаксиса и логики написан грамотно. Но, если клиент наберет 0, произойдет сбой системы.

## Компиляционный тип
Встречается при разработке на языках высокого уровня. Во время преобразований в машинный тип «что-то идет не так». Причиной служат синтаксические ошибки или сбои непосредственно в компиляторе.

Наличие подобных неполадок делает бета-тестирование невозможным. Компиляционные ошибки устраняются при разработке-отладке.

## Ресурсные
Ресурсный тип ошибок – это сбои вроде «переполнение буфера» или «нехватка памяти». Тесно связаны с «железом» устройства. Могут быть вызваны действиями пользователя. Пример – запуск «свежих» игр на стареньких компьютерах.

Исправить ситуацию помогают основательные работы над исходным кодом. А именно – полное переписывание программы или «проблемного» фрагмента.

## Взаимодействие
Подразумевается взаимодействие с аппаратным или программным окружением. Пример – ошибка при использовании веб-протоколов. Это приведет к тому, что облачный сервис не будет нормально функционировать. При постоянном возникновении соответствующей неполадки остается один путь – полностью переписывать «проблемный» участок кода, ответственный за соответствующий баг.

Источник - https://otus.ru/journal/vidy-oshibok-programmnogo-obespecheniya-bagi/#%D0%92%D0%B7%D0%B0%D0%B8%D0%BC%D0%BE%D0%B4%D0%B5%D0%B9%D1%81%D1%82%D0%B2%D0%B8%D0%B5



# Методы отладок

Отладка — этап разработки компьютерной программы, на котором обнаруживают, локализуют и устраняют ошибки. Чтобы понять, где возникла ошибка, приходится:

•узнавать текущие значения переменных;
•выяснять, по какому пути выполнялась программа.

Существуют две взаимодополняющие технологии отладки:

•Использование отладчиков — программ, которые включают в себя пользовательский интерфейс для пошагового выполнения программы: оператор за оператором, функция за функцией, с остановками на некоторых строках исходного кода или при достижении определённого условия.

•Вывод текущего состояния программы с помощью расположенных в критических точках программы операторов вывода — на экран, принтер, громкоговоритель или в файл. Вывод отладочных сведений в файл называется журналированием.

Источник - https://ru.wikipedia.org/wiki/%D0%9E%D1%82%D0%BB%D0%B0%D0%B4%D0%BA%D0%B0_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D1%8B










# Методы тестирования
















