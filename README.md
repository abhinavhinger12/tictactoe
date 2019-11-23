# tictactoe
Speech based TicTacToe based on Hidden Markov Models(HMM)
### Project Files are uploaded [Here](https://drive.google.com/file/d/1PhBFlskNBODuQeThn7-76OiSvONrNQMH/view)

## Basic Flow
1. The game will start only after either one of the user utters a specific word 'BEGIN'.
2. Each utterance of the user will be considered only after a 'green signal' is displayed to the user, which will work as a marker.
3. The game begins by showing 9 blank images corresponding to the 9 grid positions in the game and player with 'X' mark starts. 
4. Both the players speak and hence play alternately, as in the game, with 'X' and 'O' symbol assigned to them accordingly.
5. A player's turn comprises of uttering a single grid-position (from 1-9) to be marked, followed by a confirmation from the application side, to which he/she replies either 'yes' or 'no'. 
6. At this very point, there will also be a manual option available to the user for selecting the position index which acts as a 'failsafe' option, in case the postion digit is not detected after many repeated tries.
7. If 'Yes' is detected and the spoken digit position is valid, then the game smoothly proceeds ahead. 
8. While, if 'no' is detected or the spoken position is invalid, in the sense that that position was already covered or out of the scope of the game, then the given turn is repeated for that player until he utters a valid 'yes' in future or selects the position manually.
9. After each successful turn, the corresponding image (only) for that position is updated on the app screen according to the mark represented by the player of that turn.
10. Also, any user can say 'Pause' at any valid point of time during the game for pausing the game. After that, 3 options are shown to the user - 'Resume', 'Restart' & 'Quit'. The user can speak any one of them for executing it.
11. 'Resume' : resumes the game, 'Restart' : restarts the whole game afresh from the beginning, and 'Quit' : ends the game completely.


## Models created
Since this is a 2 player game, we developed 2 voice models for each word listed below. Turn alternates between 2 players and appropriate model is applied for recognition.
1. Begin
2. Digits : 0-9
3. Yes
4. No
5. Pause
6. Resume
7. Restart
8. Quit


