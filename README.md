# Battleship Game

Most everyone has played game _Battleship_. If you've never played, check out [this link](www.something.com) for a summary.

Traditionally, the grid of play is something like this:

|     | A   | B   | C   | D   | E   | F   | G   |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1   |     |     |     |     |     |     |     |
| 2   |     |     |     |     |     |     |     |
| 3   |     |     |     |     |     |     |     |
| 4   |     |     |     |     |     |     |     |
| 5   |     |     |     |     |     |     |     |
| 6   |     |     |     |     |     |     |     |
| 7   |     |     |     |     |     |     |     |

In this version, instead of the spreadsheet-esque setup with players calling "C5," you use vocab words instead:

|          | perro | gato | gallino | caballo | zapo | pollo | pato |
| -------- | ----- | ---- | ------- | ------- | ---- | ----- | ---- |
| rojo     |       |      |         |         |      |       |      |
| verde    |       |      |         |         |      |       |      |
| amarillo |       |      |         |         |      |       |      |
| negro    |       |      |         |         |      |       |      |
| blanco   |       |      |         |         |      |       |      |
| gris     |       |      |         |         |      |       |      |
| azul     |       |      |         |         |      |       |      |

Instead of telling your opponent "B3" to check a space, you say "pollo / negro" if it was a Spanish board , or "MVC / arrow function" if it were a web development board.

## GitHub Issues Setup

### Create Accounts

-   instructor's have their own "teacher" login
-   students have their own "student" logins
    -   option to have "picture" login, wheer students select a series of images?

### Instructors Create Class Data

-   Student Data
    -   instructors can copy/paste student names into an online roster 
    -   instructors can pair up students to play each other

### Instructors can determine the game setup

-   Instructors:
    -   choose the size of the board (from 3x3 up to 8x8? TBD)
    -   determine the sizes and number of ships, i.e. how many squares long for each
    -   choose vocabulary lists for
        -   rows
        -   columns

### As a player-user

-   I have ability to choose the placement of ships on my grid before the game begins

-   I see 2 grids on my screen:
    -   "my ships"
    -   "enemy ships"

### As a user during the game

-   When opponent calls the coordinates to attack, they click on that square on their board. The other player needs to click on the matching square
-   square grids change colors according to "hits" and "misses" on both the "my ships grid" and the "enemy ships grid"
-   ships change to a different color when they are sunk
