# Battleship Game

## Game Explanation

Battleship is a popular boardgame in the US. If you've never played, check out [this link](https://www.thesprucecrafts.com/the-basic-rules-of-battleship-411069) for a summary.

After secretly positioning their ships, players take turns guessing an XY coordinate on their opponent's board, and the other player tells them if it is a "hit or "miss." The game is over when one side's ships are all sunk.

<p style="font-size: 0.9rem;font-style: italic;"><img style="display: block;" src="https://live.staticflickr.com/1961/45547345711_e2701f67b0_b.jpg" alt="The Board Game of Battleship"><a href="https://www.flickr.com/photos/30478819@N08/45547345711">"The Board Game of Battleship"</a><span> by <a href="https://www.flickr.com/photos/30478819@N08">wuestenigel</a></span> is licensed under <a href="https://creativecommons.org/licenses/by/2.0/?ref=openverse&atype=html" style="margin-right: 5px;">CC BY 2.0</a><a href="https://creativecommons.org/licenses/by/2.0/?ref=openverse&atype=html" target="_blank" rel="noopener noreferrer" style="display: inline-block;white-space: none;margin-top: 2px;margin-left: 3px;height: 22px !important;"><img style="height: inherit;margin-right: 3px;display: inline-block;" src="https://search.creativecommons.org/static/img/cc_icon.svg?image_id=f470f047-1729-426c-807f-1a1f6a370acd" /><img style="height: inherit;margin-right: 3px;display: inline-block;" src="https://search.creativecommons.org/static/img/cc-by_icon.svg" /></a></p>

<p style="font-size: 0.9rem;font-style: italic;"><img style="display: block;" src="https://live.staticflickr.com/1333/1363094393_0a8809b006_b.jpg" alt="Battleship Game"><a href="https://www.flickr.com/photos/28446991@N00/1363094393">"Battleship Game"</a><span> by <a href="https://www.flickr.com/photos/28446991@N00">jking89</a></span> is licensed under <a href="https://creativecommons.org/licenses/by/2.0/?ref=openverse&atype=html" style="margin-right: 5px;">CC BY 2.0</a><a href="https://creativecommons.org/licenses/by/2.0/?ref=openverse&atype=html" target="_blank" rel="noopener noreferrer" style="display: inline-block;white-space: none;margin-top: 2px;margin-left: 3px;height: 22px !important;"><img style="height: inherit;margin-right: 3px;display: inline-block;" src="https://search.creativecommons.org/static/img/cc_icon.svg?image_id=2a6ab5a3-3717-4bef-bf35-2899c2a8aaf6" /><img style="height: inherit;margin-right: 3px;display: inline-block;" src="https://search.creativecommons.org/static/img/cc-by_icon.svg" /></a></p>

### Ships Adapted Into Candy Bars

Instead of launching missiles and sinking ships, our players will try to eat their opponent's desserts.

| Traditional Ship Name | Dessert Idea Substitute | Size of Dessert by Number of Holes |
| --------------------- | ----------------------- | ---------------------------------- |
| Carrier               | Candy Bar               | 5                                  |
| Battleship            | Popsicle                | 4                                  |
| Cruiser               | Pretzel                 | 3                                  |
| Submarine             | Baklava                 | 3                                  |
| Destroyer             | Bubble Gum              | 2                                  |

### Grid References Adapted to Use Vocabulary Words

Traditionally, the grid of play is something like this. We've marked an "X" in F3, and an "O" in B6.

|     | A   | B   | C   | D   | E   | F   | G   |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1   |     |     |     |     |     |     |     |
| 2   |     |     |     |     |     |     |     |
| 3   |     |     |     |     |     | X   |     |
| 4   |     |     |     |     |     |     |     |
| 5   |     |     |     |     |     |     |     |
| 6   |     | O   |     |     |     |     |     |
| 7   |     |     |     |     |     |     |     |

Instead of the "spreadsheet-esque" letter/number combination, (e.g. "F3") we will use vocab words. Students will say "pollo amarillo" instead of F3. Instead of "B3," you say "gato gris." Spanish vocab is used in this example, but it could easily work for any subject.

|          | perro | gato | gallino | caballo | sapo | pollo | pato |
| -------- | ----- | ---- | ------- | ------- | ---- | ----- | ---- |
| rojo     |       |      |         |         |      |       |      |
| verde    |       |      |         |         |      |       |      |
| amarillo |       |      |         |         |      | X     |      |
| negro    |       |      |         |         |      |       |      |
| blanco   |       |      |         |         |      |       |      |
| gris     |       | O    |         |         |      |       |      |
| azul     |       |      |         |         |      |       |      |

## GitHub Issues

_The GitHub issues below define project scope and goals._

### Account Management

#### Tech Needed for Authentication

-   Express
-   Handlebars
-   Node
-   password hashing
    -   does passport.js include password hashing?
    -   bcrypt if not included in passport.js
-   authentication options
    -   passport.js (library incorporates json web tokens and OAuth)
    -   do it from scratch with json web tokens (JWT) [Node.js with Passport Authentication](https://www.youtube.com/watch?v=7nafaH9SddU)
    -   OAuth- could allow Google logins
        -   OAuth = protocol
        -   AuthO = a company
-   need regex [Omar-recommended tutorial: What is Regex?](https://www.youtube.com/watch?v=r6I-Ahc0HB4)

#### Instructor Accounts

Authentication vs. Authorization will be tricky

-   authentication = allowing people to access a different part of the application
-   Instructors have their own "teacher" admin-level login
-   Teachers can create and save class rosters
    -   Teachers may Copy/paste class rosters from a spreadsheet or document to populate player lists
    -   App will save list(s) of student names for instructors to re-access once they log back in
-   Teachers can group students in various ways:
    -   class
    -   grade
    -   school

#### Student Accounts

-   students create their own "student" logins
    -   option to have "picture" login, where students select an image or series of images?

### Gameplay

#### Gameplay Tech Needed

-   drag/drop functionality
    -   HTML 5 has drag/drop API, but look on NPM
        -   sortablejs
        -   dragula
    -   don't use jQuery for drag/drop. Learn e.g. React in near future

#### Game Setup by Instructor

The instructor will...

-   choose the size of the board (from 5x5 up to 10x10? TBD)
-   determine the sizes and number of desserts, e.g. their shapes and how many squares long for each
-   choose vocabulary lists for
    -   rows
    -   columns
-   assign students to games

### Student/Player Game Setup

As a student/player...

-   I can play other students online
-   I have ability to choose the placement of ships on my grid before the game begins
    -   I can rotate the
-   I see 2 grids on my screen:
    -   "my ships"
    -   "enemy ships"

### As a user during the game

-   When opponent calls the coordinates to attack, they click on that square on their board. The other player needs to click on the matching square
-   square grids change colors according to "hits" and "misses" on both the "my ships grid" and the "enemy ships grid"
-   ships change to a different color when they are sunk
