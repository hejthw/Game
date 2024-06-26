# Operation: Intrude 

**Платформа**:

Windows

**Технологии**:

Godot

**Язык**: 

Русский

**Жанр**:

Стелс-экшен

**Сеттинг**:

Наше время

**Длительность игры**:

15 мин.

# Cюжет
Игрок берет под контроль оперативника, задача которого незаметно проникнуть на базу врага чтобы украсть или саботировать разработку, которая может повлиять на ход сражения.



# Игровой мир
Действие игры происходит на секретной базе врага. В ходе игры игрок проникает на базу, минуя врагов.

# Геймплей
2D Статичный вид сверху.

Цель игры проходить "экраны" комнаты базы не попадая в поле зрения врага.

Пример "экрана":

![aa](https://github.com/hejthw/Game/blob/main/readme.img/Mgear.png)

При обнаружении игрока срабатывает тревога, приводящая врагов на экране к режиму боя, из-за которого они начинают атаковать игрока.

Игроку доступен рукопашный бой и огнестрельное оружие для нейтрализации врагов

По базе разбросаны предметы, помогающие игроку в прохождении.


# Сущности

## Враги:

**Примечание**:

У каждого врага имеется поле зрения в виде конуса, отвечающее за обнаружение игрока.

**Пример поле зрения**:

![aa](https://github.com/hejthw/Game/blob/main/readme.img/81WLT.png)

где синий круг - враг, оранжевый конус - его поле зрения, 

**Виды врагов**:

1)Охранник - сущность патрулирующая определенный маршрут на экране. Может быть нейтрализован на несколько секунд с помощью рукопашного боя или полностью уничтожен с помощью огнестрельного оружия.

2)Камера - недвижимая сущность располагающаяся на стене. Не может быть уничтожена игроком.

## Пикапы

По ходу прохождения игрок сможет найти на локациях предметы расположенные на земле - "Пикапы"

**Виды пикапов**:

1) Глушитель - надевается сразу при поднятии игроком, расходуемый предмет, глушит звук оружия игрока, позволяя использовать огнестрельное оружие без поднятия тревоги.

2) Патроны - используется сразу при поднятии игроком, восполняет запас патронов основного оружия игрока на 6 шт.

3) Аптечка - используется сразу при поднятии игроком, полностью восполняет здоровье игрока.

4) Ключ-карта - ключевой предмет, который в некоторых ситуациях потребуется для дальнейшего прохождения.

# Взаимодействия

## **Ввод игрока**:

WASD - Управление персонажем

G - Рукопашный бой

Space - Выстрел из огнестрельного оружия


## **Игрок-враг**:

Попадание игроком рукопашной атакой - вывод из строя врага на 15 секунд.

Попадание игроком огнестрельной атакой - убивает врага.

## **Враг-игрок**:

Попадание в поле зрения - активация режима боя

Попадание вражеской сущности по игроку - нанесение урона в 50% 


