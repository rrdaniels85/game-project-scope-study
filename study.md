# Game Project Scope Study

## Required Readings

-   [Game Project](https://github.com/ga-wdi-boston/game-project)
-   [Game API](https://github.com/ga-wdi-boston/game-project-api)
-   [What is a User Story](https://www.mountaingoatsoftware.com/agile/user-stories)

## Deliverables

After reading the `game-project` prompt and the `game-project-api` documentation
please do the following and be prepared to share and discuss during our next
class.

Submit detailed answers to the following in this file via a pull request:

-   A wireframe of what your game project will look like.
    -See images
    [Wireframes](http://imgur.com/a/kPpbs)
-   The data structure you plan to use.
  - For my Ajax communications with the server, I plan to use the JSON data structure. The documentation we've received makes it clear how the data needs to be structured in the JSON so that I successfully can communicate with the back end through Ajax requests. For example, a player move would need to be structured as such for me to communicate it to the back end: {
  "game": {
    "cell": {
      "index": 0,
      "value": "x"
    },
    "over": false
  }
}
-   How you will take the markup of the game board and represent it in JS
    - I hope to use HTML and CSS to make the tic tac toe game board with 9 different divs. Each div will be given an ID that will go 0 through 8. I plan to represent the game board in JS in the form of an array with nine indexes. Each index in the array represents one of the tic tac toe squares. I will put in an event handler so that when a user clicks on one of the divs, the ID associated with that div will be used to assign a value to that same position in the JS array of either X or O depending on which player clicked on the div. This will allow me to keep track of the game and check for winning combinations.
-   How you plan to approach this project.
  - First - I plan to create a repository for the front-end of my app. Then, I will create my basic HTML/CSS structure of the game board. Then I plan to write out my JS logic (ex. how the game board will be filled out, wins vs. draws determined, etc.) I will then link my javascript with the DOM through JQuery and allow the two to interact. Finally, I will hook up all the JQuery and logic to the back end through Ajax. Once the basic requirements of the project are met, I then plan to pursue some of the bonus challenges.
-   4-8 user stories for your game project.
  - 1) As a user, I want sign in and sign up fields with clear labels so that I can sign in or sign up to play games on the website.
  - 2) As a user, I want a properly labeled and functioning new game button so that I can begin a new tic tac toe game when I click on it.
  - 3) As a user, when I click on a particular square on the game board, I want the correct corresponding token to appear there so that I and the other player can see where I made a move.
  - 4) As a user, when a player has played a winning combination of game board squares, I want the app to notify me so that I am aware which player has won.
  - 5) As a user, when a player achieves a winning combination, I want the game to end.
  - 6) As a user, if all the squares have been played and no winning combination has been achieved, I want the app to notify the players so that I am aware that the game ended in a draw.
  - 7) As a user, when I click the new game button, I want a new game board to appear so that I can begin a new game.
  - 8) As a user, when I win a game, I want that game to be recorded and my past game history to be updated so that I know how many games that I have won in total.
-   How you plan to keep your code modular.
    - I will be sure that there are separation of concerns in my code, particularly with regard to interactions with the back end. For example, I will have an events.js file which will house my code related to my event handlers. I will also have a separate file for communication with the API using Ajax. My main game board javascript game logic will also be separated from these other pieces. I will keep my initial index.html and css pages separate as well. By doing this, I think it will be easier to keep track of my code and test it as I go.
-   What creative spin will you add to your project?
    - I want to include some sort of fun theme that either goes along with just the
    Xs and Os (ex. football, valentine's day) or the player can customize their tokens to correlate with some random theme that I style the board to go along with (ex. Star Wars - Jedis vs. Sith). I have not yet decided on my final theme.
-   How will you use version control to backup / track your project?
    I plan to make regular commits and pushes to github through the life of my project. It will be critical for me to put detailed and clear commit messages in with the commits so that if I need to load or review any past versions, it will be easy for me and others to understand in the future what I did at various points in the project.
-   Do you plan to attempt any of the bonuses?
    - Yes, there are a number that I am interested in. However, the main ones that I hope to include will be keeping track of multiple game rounds with a win counter and allowing players to customize their tokens.

You may want to submit pictures for your wireframes and/or user stories.
[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
has instructions to link to a picture you've uploaded to a service like [Imgur](http://imgur.com/).
