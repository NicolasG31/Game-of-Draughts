Game of Draughts


Design Decisions:

The Game of Draughts application follows a standard board game desktop application pattern. We can cut this pattern into 3 distinct parts:
The Board

The main purpose of the program is to play a board game, so we decided to let the board occupy a major part of the game window. The game board starts initialized by default, we want the user to begin to play as fast as possible when he launches the program. Our game is the game of Draughts, so we have to differentiate two players, and therefore we have chosen two "opposite" colors: white and red. The board cells have two colors as well, grey and green, so they mismatch the colors of the pawns. These colors form a grid to easily differentiate the cells.

When a player clicks on one of his pieces, the cell he has selected is highlighted to show the user has selected the associated pawn. We thought the user would be more satisfied if the click had a visual response. The more interactive our UI would be, the better it would be. Then, if the selected pawn could move somewhere on the board, we draw the possible moves as hints on the cells the user could click on. We give these hints to the users so they know what to do, and know what is the expected behavior.
Game Status

Next to our board on the left is set an area where informations about the current game are displayed. We can notice there are two distinct parts, each part corresponding to a player, the red and the white one. Below the associated pawn, there are two variables. The score of the actual player, which is defined by how many pieces of the opponent he has eaten, and the number of jumps, simply said moves, he has done. The font is simple and written uppon a plain color to make it easy to read. Now let's say it's the red player's turn to play. A highlighted text will appear under the two variables telling it's his turn to play. We chose to make this text big and blue highlighted so we can easily tell which player's turn it is. We can also see that the font is bigger then the score and jumps text, so it really stands out. When the game is over, the same blue highlighted label is displayed under the winner of the game, which produces the same effect and highlights the winner. If there is no winner, we display the same label under the two players to show it's a draw.
The Menu Bar

At the top left is located the menu bar. This is the place where we expect the menu to be. The menu is quite simple, first we have the possibility to restart the game. This action will simply reset our board and restart the status of the game. The user can choose to do it at the end of the game or simply whenever he wants to. The second action is to simply quit the program. These two actions have assigned shortcuts, so the user can perform them quicker if he knows them. 