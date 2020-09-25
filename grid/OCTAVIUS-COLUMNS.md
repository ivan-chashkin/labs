#  Заметки про колонки в layout octavius

Нужно реализовать пользовательский resize колонок. Также по возможности ускорить рендерин при ресайзе окна.

## И так имеем
Входы: ширина экрана, Xpane, Xview, текущий роут (в результатах поиска папки фиксированно отображаются)

### 2pane
#### Обычный вид
[0,761]
Колонка     Ширина      Тянется
Контейнер   761px       -
left-column             64px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            0           -

(762,960]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             64px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            0px         -

(960,1200]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             64px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            168px       -

(1200,1260]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             232px       -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            168px       -

(1260,1800]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             232px       -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            248px       -

(1800,2150]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             272px       -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            248px       -

(2150,Infinity)
Колонка     Ширина      Тянется
Контейнер   2150        -
left-column             272px       -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            248px       -

### 2pane
#### Компактный вид
[0,761]
Колонка     Ширина      Тянется
Контейнер   761px       -
left-column             56px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            0           -

(762,960]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             56px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            0px         -

(960,1200]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             56px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            168px       -

(1200,1260]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             232px       -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            168px       -

(1260,1800]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             232px       -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            248px       -

(1800,2150]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             252px       -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            248px       -

(2150,Infinity)
Колонка     Ширина      Тянется
Контейнер   2150        -
left-column             252px       -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            248px       -

### 3pane
#### Обычный вид
[0,761]
Колонка     Ширина      Тянется
Контейнер   761px       -
left-column             64px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            0           -

(762,960]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             64px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            0px         -

(960,1200]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             64px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            168px       -

(1200,1260]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             64px        -
main-frame-sidebar      280px       -
main-frame-content      auto        +
right-column            168px       -

(1260,1420]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             232px       -
main-frame-sidebar      320px       -
main-frame-content      auto        +
right-column            248px       -

(1420,1800]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             232px       -
main-frame-sidebar      400px       -
main-frame-content      auto        +
right-column            248px       -

(1800,1920]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             232px       -
main-frame-sidebar      400px       -
main-frame-content      auto        +
right-column            248px       -

(1920,2150]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             272px       -
main-frame-sidebar      400px       -
main-frame-content      auto        +
right-column            248px       -

(2150,Infinity)
Колонка     Ширина      Тянется
Контейнер   2150        -
left-column             272px       -
main-frame-sidebar      400px       -
main-frame-content      auto        +
right-column            248px       -

### 3pane
#### Компактный вид
[0,761]
Колонка     Ширина      Тянется
Контейнер   761px       -
left-column             56px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            0           -

(762,960]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             56px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            0px         -

(960,1200]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             56px        -
main-frame-sidebar      auto        +
main-frame-content      0           -
right-column            168px       -

(1200,1260]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             56px        -
main-frame-sidebar      280px       -
main-frame-content      auto        +
right-column            168px       -

(1260,1420]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             56px       -
main-frame-sidebar      320px       -
main-frame-content      auto        +
right-column            168px       -

(1420,1800]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             232px       -
main-frame-sidebar      320px       -
main-frame-content      auto        +
right-column            248px       -

(1800,1920]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             232px       -
main-frame-sidebar      400px       -
main-frame-content      auto        +
right-column            248px       -

(1920,2150]
Колонка     Ширина      Тянется
Контейнер   auto        +
left-column             252px       -
main-frame-sidebar      400px       -
main-frame-content      auto        +
right-column            248px       -

(2150,Infinity)
Колонка     Ширина      Тянется
Контейнер   2150        -
left-column             252px       -
main-frame-sidebar      400px       -
main-frame-content      auto        +
right-column            248px       -


left-column
    2pane / обычный вид
    [0,761] (762,960] (960,1200]: 64px
    (1200,1260] (1260,1800]: 232px
    (1800,2150] (2150,Infinity): 272px

    2pane / Компактный вид
    [0,761] (762,960] (960,1200]: 56px
    (1200,1260] (1260,1800]: 232px
    (1800,2150] (2150,Infinity): 252px

    3pane / Обычный вид
    [0,761] (762,960] (960,1200] (1200,1260]: 64px
    (1260,1420] (1420,1800] (1800,1920]: 232px
    (1920,2150] (2150,Infinity): 272px

    3pane / Компактный вид
    [0,761] (762,960] (960,1200] (1200,1260] (1260,1420]: 56px
    (1420,1800] (1800,1920]: 232px
    (1920,2150] (2150,Infinity): 252px

