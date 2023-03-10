# Day 01 – Введение в анализ данных
## Оглавление
1. [Глава I](#глава-i) \
    1.1. [Преамбула](#преамбула)
2. [Глава II](#глава-ii) \
    2.1. [Общая инструкция](#общая-инструкция)
3. [Глава III](#глава-iii) \
    3.1. [Цели](#цели) 
4. [Глава IV](#глава-iv) \
    4.1. [Задание](#задание)
5. [Глава V](#глава-v) \
    5.1. [Сдача работы и проверка](#сдача-работы-и-проверка)

## Глава I
### Преамбула
За последние годы Язык Программирования (ЯП) Python стал первоклассным инструментом для анализа и визуализации
больших массивов данных. За счет его читабельности, простого синтаксиса и отсутствия необходимости в компиляции,
язык хорошо подходит для обучения программированию, позволяя концентрироваться на изучении алгоритмов, концептов и парадигм.
Python занимает первое место в рейтинге самых популярных ЯП [TIOBE](https://ru.wikipedia.org/wiki/%D0%98%D0%BD%D0%B4%D0%B5%D0%BA%D1%81_TIOBE).

Популярность ЯП Python именно для науки о данных обусловлена прежде всего большой и активной экосистемой библиотек:
- **NumPy** для работы с однородными массивами данных, 
- **Pandas** для работы с разнородными и помеченными данными, 
- **SciPy** для решения общих задач научных вычислений, 
- **Matplotlib** для визуализаций качества публикации, 
- **Scikit-Learn** для машинного обучения
- **Pytorch** для нейронных сетей \
и многие другие инструменты, с которыми мы познакомимся по ходу курса. Но сначала мы должны хотя бы немного погрузиться в ЯП Python.

## Глава II
### Общая инструкция

Методология Школы 21 может быть не похожа на тот образовательный опыт, который с вами случался ранее. 
Ее отличает высокий уровень автономии: у вас есть задача, вы должны ее выполнить. 
По большей части вам нужно будет самим добывать знания для ее решения. Второй важный момент – это peer-to-peer обучение. 
В образовательном процессе нет преподавателей и экспертов, перед которыми вы защищаете свой результат. 
Вы это делаете перед такими же учащимися, как и вы сами. 
У них есть чек-лист, который поможет им выполнить приемку вашей работы качественно.

Роль Школы 21 заключается в том, чтобы обеспечить через последовательность заданий и оптимальный уровень поддержки 
такую траекторию обучения, при которой вы освоите не только hard skills, но и научитесь самообучаться.

* Не доверяйте слухам и предположениям о том, как должно быть оформлено ваше решение. Этот документ является единственным источником, к которому стоит обращаться по большинству вопросов.
* Ваше решение будет оцениваться другими учащимися.
* Подлежат оцениванию только те файлы, которые вы выложили в GIT, ветка  develop, папка src.
* В вашей папке не должно быть лишних файлов – только те, что были указаны в задании.
* Есть вопрос? Спросите коллегу справа. Не помогло? Спросите коллегу слева.
* Не забывайте, что у вас есть доступ к интернету и поисковым системам.
* Обсуждение заданий можно вести и в Slack.
* Будьте внимательны к примерам, указанным в этом документе – они могут иметь важные детали, которые не были оговорены другим способом.
* И да пребудет с вами Сила!

## Глава III
### Цели
Целью этого проекта является дать вам базовое понимание синтаксиса, основных конструкций и 
возможностей ЯП [Python](https://www.python.org/). Также вы познакомитесь с интерактивной 
средой разработки [Jupyter](https://jupyter.org/).

## Глава IV
### Задание

Для начала настрой свою рабочее окружение: 
* Установи и настрой Jupyter.
* Открой файл 01-intro.ipynb. Познакомься с основами синтаксиса языка Python.
* Открой файл 01-assigment.ipynb и приступай к выполнению задания

### Task 1
Напиши формулу нахождения корней квадратного уравнения на языке LaTeX.\
Затем напиши функцию, которая будет решать квадратное уравнение:
- Функция принимает на вход коэффициент a, b, c. 
- Функция должна возвращать кортеж корней уравнения.
- Если корней у уравнения нет, то функция должна вернуть ```None```

### Task 2
Напиши функцию, которая на вход будет принимать список случайных чисел, а возвращать уже отсортированный по возрастанию. \
Для сортировки используй самую простую сортировку чисел - [Сортировку Пузырьком](https://ru.wikipedia.org/wiki/%D0%A1%D0%BE%D1%80%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%BA%D0%B0_%D0%BF%D1%83%D0%B7%D1%8B%D1%80%D1%8C%D0%BA%D0%BE%D0%BC). Псевдокод алгоритма описан в статье. \
Для удобства тестирования корректности работы функции, сгенерируй случайную последовательность чисел с помощью стандартной библиотеки random.

### Task 3
Найди самое часто встречающееся слово в романе "Война и Мир".
Из подсчета исключи:
- Пунктуацию
- Слова **короче четырех** символов
- 'Стоп-слова', которые приведены в [файле](materials/stop_words_russian.txt)

Обязательно поделитесь с пирами в Slack сколько раз у вас встретилось это слово. Результаты, в зависимости от предобработки, могут чуть отличаться.

### Task 4
Напиши функцию для расчета числа Фибоначчи. В реализации **используй рекурсивную функцию**.

### Task 5
Напиши функцию для перевода валюты в рубли. 
На вход функция принимает название валюты (EUR, USD, GBP) и ее объем, а возвращает стоимость в рублях.  
Для получения актуальных курсов валют самостоятельно изучите библиотеку requests и обработайте ответ от этого [этого сервиса](https://www.cbr-xml-daily.ru/daily_json.js) (Ответ приходит в JSON формате)

### *Task 6. Дополнительное задание
Кроме самого синтаксиса ЯП также важно знать Алгоритмы и структуры данных. Это очень обширная тема. В университете она по-хорошему читается курса 4 :) Понятно, что в данном курсе времени меньше, но не рассказать про нее все равно нельзя.

Знание алгоритмов и структур данных поможет реализовывать в коде более удачные по времени работы и потребляемой памяти решения, а в некоторых случаях — справляться с теми задачами, с которыми без знания алгоритмов не получится справиться вовсе. Ну и на собеседованиях написание алгоритмов - любимая тема. Попробуй реализовать наверное одну из самых популярных задач на собеседованиях - Написание проверки на пaлиндром:
- На вход функции isPalindrome подается число (int). 
- Функция возвращает True, если число является палидромом и False в противном случае. 
- Реализуй функцию двумя способами:
    - с переводом числа в строку
    - без перевода числа в строку 

Дополнительные ресурсы для обучения мы привели в файле [reading_list.md](materials/reading_list.md) \
Если же вы хотите поделиться с сокурсниками еще какими-либо полезными материалами по теме - **смело пишите их в чат проекта!**

Также в файле [helpful.ipynb](code-samples/helpful.ipynb) можно найти полезные для выполнения задания функции.

## Глава V
### Сдача работы и проверка
Сохраните решение в файле 01-assignment.ipynb\
Загрузите изменения на Git в ветку develop.



💡 [Нажми здесь](https://forms.gle/7Yte6UwKLWobEm3j6) **чтобы отправить обратную связь по проекту**. 

