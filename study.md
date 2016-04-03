# Game Project Scope Study

## Required Readings

-   [Game Project](https://github.com/ga-wdi-boston/game-project)
-   [Game API](https://github.com/ga-wdi-boston/game-project-api)
-   [What is a User Story](http://searchsoftwarequality.techtarget.com/definition/user-story)

## Deliverables

After reading the `game-project` prompt and the `game-project-api` documentation
please do the following and be prepared to share and discuss on Monday morning.

Submit detailed answers to these in this file via a pull request.

-   A wireframe of what your game project will look like.
-   The data structure you plan to use.
-   How you will take the markup of the game board and represent it in JS
-   How you plan to approach this project.
-   4-8 user stories for your game project.
-   How you plan to keep your code moodular.
-   What creative spin will you add to your project.
-   How you will use version control to backup / track your project.
-   Do you plan to attempt any of the bonuses.

## Project Components

### Wireframe

http://imgur.com/a/YBlKy

### Data Structure

I plan to use an array with each square of the board being represented by an index position (0-8).  I will use jQuery to allow the user to interact with the board via click handlers, reset the board, sign up for an account and manage their account.      

### Representation of Markup

Wins will result when 3 indices of X/O align as per the game rules.  For example, a diagonal X win case could be (board[0] === 'X' && board[4] === 'X' && board[8] === 'X').  Tie cases will result when each index of the array is either X or O.

### Approach

First I will re-read the documentation (project requirements and the game API).  I plan to closely follow the suggestions for what to do and in what order as outlined in the game-project repository.  Specifically, I will:

--   Create a simple HTML layout and style it it with CSS.
--   Design the game logic in JS.
--   Add jQuery code to allow user interaction with the game
--   Add jQuery code to allow user interaction with the account features
--   Write curl requests to the test api.
--   Add AJAX code.

If I find myself spending an inordinate amount of time on a step that is sufficiently complete but could be somewhat improved for aesthetic purposes I will remind myself to move on and return to it only when I have satisfied all other criterion of the project.  I will also do my best to allocate sufficient time for steps that I anticipate will be more difficult for me than others, like writing jQuery to handle browser interaction.

At all steps I will test my code using the techniques we've learned (console.log, debuggers, httpbin.org etc).

### User Stories

1.  As a user, I want to be able to sign up so I create an account and sign in.
1.  As a user I want the square that I click to populate with X or O so I can have my move registered.
1.  As a user, if I win or tie I want to see a message to that affect so I know the game's outcome.
1.  As a user, I want to be able to see the amount of wins for X and Y and the number of ties so I can keep track of previous matches.
1.  As a user, I should be able to change my password to manage my account.
1.  As a developer, I want to test my code frequently in the interest of minimizing errors.

### Code Modularity

To prevent redundant coding I will stick to the principles of DRY and use techniques we have learned such as implementing callback functions.  I will also keep my code modular by storing it in separate and appropriately sized files based on the code's function.

### Creative Spin

I thought about creating a themed app but I think it's better for me to focus on creating a simple, clean layout.  I plan on exercising my creativity in making that layout visually appealing and possibly creating different icons other than just X's and O's.  If I have extra time I will try to implement more advanced CSS styling.

## Version Control

To backup/track my project, I will make frequent and descriptive commits to my project repository.

## Bonus Plans

I am not planning to attempt any of the bonuses barring a (possible) JQuery epiphany.
