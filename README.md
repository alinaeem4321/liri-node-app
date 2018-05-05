**How liri-node-app works**
Type the following 4 commands in terminal/bash window and result will show up on terminal/bash window and also in Log.txt file which logs all the commands :-
1. `node liri.js my-tweets`
    * It will print all my tweets in bash window and also log them in log.txt file
    * Currently I have only 15 tweets, but it can pull 20 tweets, if I add more tweets.
    
2. `node liri.js spotify-this-song '<song name here>'`
    * If no song is provided then your program will default to "The Sign" by Ace of Base. * The album that the     song is from*.
    * User can also find more than one song related to their search parameters if tyey type in number of songs they want and what topic they want the song to be about. like if the user types
    `node liri.js spotify-this-song 3 love'`will out put 3 songs about love. 
    * This will show the following information about the song in your terminal/bash window  
     * Artist(s)
     * The song's name 
     * A preview link of the song from Spotify

3. `node liri.js movie-this '<movie name here>'`
   * If the user doesn't type a movie name, the program will output data for the movie 'Mr. Nobody.'
   * Example: User can type in as `node liri.js movie-this Lion King'`, and the program will print,
   * This will output the following information to your terminal/bash window:
       * Title of the movie.
       * Year the movie came out.
       * IMDB Rating of the movie.
       * Rotten Tomatoes Rating of the movie.
       * Country where the movie was produced.
       * Language of the movie.
       * Plot of the movie.
       * Actors in the movie.

4. `node liri.js do-what-it-says`
   * Using the `fs` Node package, LIRI will take the text inside of random.txt and then use it to call one of LIRI's commands.
     * It should run `spotify-this-song` for "I Want it That Way," as follows the text in `random.txt`.
    * If you change the command in random.txt the program will run as what it says in the random.txt file.
    Like move-this, "Cindrella" will out put about movie Cindrella. 
    If user mistyped the command the liri will give the user an message telling that the command is not recoganized and will suggest the right commands to make liri work.