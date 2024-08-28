1. Скопирую папку `src` и бинарник `mixer` из CA_project.
2. В файле `equations.ipynb` сделаю функции для расчета уравнений поверхности, площадей и профилей плотности.

## 18.12.23

1. #Info В папке `/wolfram` хранятся файлы c всеми расчетами для wolfram mathematica
2. Сделаю файл `auxil.py`, в котором напишу все функции для расчета площадей поверхности и профилей плотности

## 10.02.24
3. Наконец-то закончил писать формулы...
4. Сделаю файли `velidation.ipynb`, где проверю формулы на предельном случае.

## 11.02.24
5. По результатам тестов
    droplet     +
    doughnut    - некоторые S_general не сходятся с S_180, min и max не сходятся
    worm        +
    roll        - сильно не сходятся S_general и S_180, все min и max сходятся
    perforation - вообще пиздец
6. Поправил doughnut
7. Поправил roll
8. Поправил perforation
9. #Success Получилось добиться нулевой ошибки между S, phi_min и phi_max
10. Добавлю еще layer
11. Сделяю файл `phase_diagram.ipynb`, где буду строить фазовые диаграммы. Часть кода возьму из старой версии `droplet_diagram.ipynb`.

## 17.02.24
12. Для каждой капли напишу функцию y(z), которая будет задавать уравнение их поверхности. На осне этих функций задам уравнение профиля плотности
13. #Success Написаны уравнения и профили для всех капелек. В половине формул из статьи Ильи найдены ошибки...

## 28.02.24
14. #Remember Перенес файл с формулами в `src/utils_py/auxil.py`.
14. Допишу в генератор регионы, которые позволят генерировать нужные капли.
15. Займусь генерацией искуственных датасетов. Для этого сделаю файл `syn_gen.ipynb`, где будет генерировать искуственный датасеты для каждого типа капель.
16. Сделю gro для простой точки `point.gro`
17. Скопирую из `CA_project` файл `profile_approx.ipynb`
18. Вместо gmx density напишу свою штуку, которая генерирует профиль плотности

## 13.03.24
19. Займусь построением графика true-predict для углов