# Русский перевод vi/vim graphical cheat sheet

В данном файле представлен перевод vi/vim graphical cheat sheet в текстовом формате, позже будет добавлена и графическая часть.

Оригинал: http://www.viemu.com/a_vi_vim_graphical_cheat_sheet_tutorial.html

Оригинал в html формате: https://loginovilya.github.io/vi-vim-graphical-cheat-sheet-ru

### Обозначения

motion - перемещает курсор или определяет диапазон для оператора  
command – команда прямого действия; если выделена жирным ( в графическом варианте красным цветом ), переводит в режим вставки  
operator  – требует движения в будущем, управляет курсором и направлением  
extra – специальные функции, требуют дополнительного ввода  
q● – команды с точкой требуют ввода знакового аргумента

слова: quux ( foo , bar , baz );  
СЛОВА: quux(foo, bar, baz);



### Кнопки
**motion**
```
`●  - метка перехода
#   - предыдущая идентификация
$   - конец строки
%   - согласование перехода
^   - в начало строки (к первому непробельному символу)
*   - следующая идентификация
(   - начать предложение
)   - закончить предложение
0   - к началу строки
_   - к началу строки вниз
-   - предыдущая строка
+   - следующая строка
W   - следующее СЛОВО
w   - следующее слово
E   - закончить СЛОВО
e   - закончить слово
T●  - назад до
t●  - до
{   - начать абзац
[●  - прочее
}   - закончить абзац
]●  - прочее
F●  - «обратный» поиск символа
f●  - поиск символа
G   - конец файла/переход строки
H   - верхняя часть экрана
h   - '←'
j   - '↓'
k   - '↑'
L   - нижняя часть экрана
l   - '→'
;   - повторить t/T/f/F
'●  - метка перехода в начало строки
|   - начало строки/переход к столбцу
B   - предыдущее СЛОВО
b   - предыдущее слово
N   - предыдущий (найти)
n   - следующий (найти)
M   - средняя часть 
,   - обратный t/T/f/F
?●  - найти (ред.)
/●  - найти
```
**command**
```
Esc - обычный режим
~   - переключение регистра
@●  - выполняет макрокоманду
&   - повтор :s
Q   - режим ex
q●  - запись макрокоманды
R   - режим замены
r●  - заменить исмвол
Y   - копировать строку
U   - вернуться на строку
u   - отменить
I   - вставить в начале строки
i   - режим вставки
O   - открыть выше
o   - открыть ниже
P   - вставить до
p   - вставить после ( 1 )
A   - добавить в конец строки
a   - добавить
S   - заменить строку
s   - заменить знак
D   - удалить в конец строки
J   - объединить строки
K   - помощь
:   - командная строка ex
X   - возврат
x   - удалить символ
C   - изменить в конце строки
V   - визуальные строки
v   - визуальный режим
m●  - поставить метку
.   – повторить команду
```
**operator**
```
!   - внешний фильтр
=   - автоформат
y   - копировать ( 1, 3 )
d   - удалить ( 1, 3 )
c   - изменить ( 1, 3 )
<   - отсутствие отступа ( 3 )
>   - отступ ( 3 )
```
**extra**
```
1    - ( 2 )
g●   - дополнительные команды ( 6 )
”●   - специальный 
\●   – не используется!
Z●   - выйти ( 4 )
z●   - дополнительные команды ( 5 )
```

### Основные команды командной строки ('ex'):
:w (сохранить), :q (выйти), :q!(выйти без сохранения)  
:e f (открыть файл f),  
:%s/x/y/g (заменить 'x' на 'y' во всем файле),  
:h (помощь в vim), :new (новый файл в vim),  

**Прочие важные команды:**  
CTRL-R: повтор (vim),  
CTRL-F/-B: на страницу вверх/вниз,  
CTRL-E/-Y: прокрутить на строку вверх/вниз,  
CTRL-V: блок-визуальный режим (только vim)  

**Визуальный режим:**  
Перемещение и ввод оператора для действий в выбранной области (только vim)


### Примечания:

 - Использовать "x" до выполнения команд копировать/вставить/удалить для использования этого регистра («буфер обмена данными») (x=a..z,*) (например: "ay$ для копировани оставшейся части строки в регистр 'a')
 - Ввести число до выполнения любого действия для повтора этого
    числа раз  (например: 2p, d2w, 5i, d4j)
 - копировать оператора для действий в текущей строке (dd =
    удалить строку, >> = выровнять строку)
 - ZZ для сохранения и выхода, ZQ для выхода без сохранения
 - zt: прокрутить курсор наверх, zb: вниз, zz: в центр
 - gg: начало файла (только vim), gf: открыть файл под курсором (только vim)

### Перевод аббревиатур из оригинала 

 - bol = начало строки
 - eol = конец строки
 - mk = метка

### Лицензия
[GNU Free Documentation License](https://en.wikipedia.org/wiki/GNU_FDL)
