# Battleship Game

## Game Explanation

Most everyone has played game _Battleship_. If you've never played, check out [this link](https://www.thesprucecrafts.com/the-basic-rules-of-battleship-411069) for a summary.

### Ships

Each player starts with these ships:

| Ship Name | Size of Ship by Number of Holes |
| --- | --- |
| Carrier | 5 |
|Battleship | 4 |
| Cruiser | 3 |
| Submarine | 3 |
| Destroyer | 2 |

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

|          | perro | gato | gallino | caballo | sapo | pollo | pato |
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
#### Instructor Accounts
-   Instructors have their own "teacher" login
-   Teachers can copy/paste class rosters to populate player lists
-   App will save list(s) of student names

#### Student Accounts
-   students have their own "student" logins
    -   option to have "picture" login, where students select an image or series of images?

### Instructors can determine the game setup

-   choose the size of the board (from 3x3 up to 10x10? TBD)
-   determine the sizes and number of ships, i.e. how many squares long for each
    -   traditionally, Battleship has 
        -   Carrier, which has five holes
        -   Battleship, which has four holes
        -   Cruiser, which has three holes
        -   Submarine, which has three holes
        -   Destroyer, which has two holes

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
