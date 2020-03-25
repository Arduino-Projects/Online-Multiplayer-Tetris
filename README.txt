There were a lot of games that I played and eventually got bored of as a kid. But I've been playing Tetris forever and I just can't get bored of it! That's why I made my own multiplayer Tetris game!




How It Works


Basically, two players join the game by going on the website that the code is hosted on. Once the game detects that two people are on, it connects them both to the game and starts! Both players are given their own tetris games, and they can see what their opponent is doing at any time!




What's The Goal


When a player clears four lines for example, then four attack lines will be added to the bottom of the opponents stack! To get rid of these attack lines, the opponent has to clear some of their own lines, and then the attack lines at the bottom of their board will disappear. This will keep going until one player's stack reaches the top, which means they lose!




How Was It Made


The game was coded in HTML and JavaScript. To get the players to be connected, and for their boards to be sent over to each other, I used FireBase!




Main Pieces of Code


There were essentially four main parts of the code

- The tetris game itself

- The game audio

- Updating and reading from the FireBase Database

- The text, and titles




The Tetris Game


The whole tetris board you see is essentially a 20x10 2D Array, or an array inside of an array. This array contains integers, each one to signify a different color. So when a person sees all the colors on the board, they start to look like pieces! The grid erases a row every time a row gets filled, and then tells the database to push the opponents stack up! The pieces move and rotate by simply moving the numbers around the 2D array, which again, looks like pieces moving and rotating to us! Once the game detects that the new piece being spawned overlaps with another piece, then it knows the player has lost. It tells the database that this player has lost, and the other player has won! This part cooperated really well with me, but it was extremely brain-consuming and tiring as its really just a bunch of weird math!




The Game Audio

This part turned out to be super tricky, as playing audio in a web browser can be very annoying!!! There are MP3 audio files for all the sound and voice effect in the project folder. Whenever a sound needs to be played, the code simply runs the play function on the audio file, and it plays the sound. I know it sounds really simple, BUT IT WAS SOOOO ANNOYING!!




The FireBase Database

Firebase is basically a service provided by Google that includes a realtime-database feature! This allows the data in that database to be updated from one player, and then the other player can see the changes within milliseconds! Incorporating this with JavaScript was also pretty tricky, but I managed to get through it! The database is updated with various things, such as each players grid array, their number of lines sent, and various other parameters. This is essentially the foundation of the two browsers talking to each other!




The Titles and Text

This was just a fun little touch up that makes the game look nicer! I added titles to label the parts of the game so that the user would know what to do and when to do it! It was the easiest part of the game!




The Final Result!

The code for the game is linked below! And the website that the game is hosted on is also linked here! All in all, this was a great way to spend 2 days of my isolation and I hope all of y'all enjoy playing my game!!




Website: https://w0egd.codesandbox.io/
