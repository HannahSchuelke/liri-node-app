# LIRIbot

In this assignment I've created a LIRI, like iPhone's SIRI, but it's a Language Interpretation and Recognition Interface rather than a Speech Interpretation and Recognition Interface. LIRI is a command line node app that takes in parameters and gives you back data. Data returned will come from Spotify for songs, Bands in Town for concerts, and OMDB for movies.

This is a Javascript/jQuery/API/NodeJS project for the UMN Coding Bootcamp, assignment 8. 

## Getting Started

To utilize this project, I access my LIRIbot files via my terminal. From there, I can search for songs, concerts, and movies via using node commands as `concert-this`, `spotify-this-song`, `movie-this`, and `do-what-it-says`.

### Prerequisites

If you would like to utilize my project, you must first do an npm install. You must also clone the files from my Github repository "liri-node-app" and source your own API keys to put in an .env file, all within the same folder. 

### Installing

1. Direct yourself to the folder where you'd like to test my project. 
2. Do an npm install. 
3. Go to https://github.com/HannahSchuelke/liri-node-app and clone my files into the same folder.
4. Make a .gitignore file and type `node_modules`, `.DS_Store`, and `.env` into it. 
5. Source your own Spotify API key and insert that in your .env file. 
6. Open up your terminal and direct yourself to the folder where you have rooted my project. 
7. From here you may find information by typing "node liri.js *function* *search string*" into your terminal/bash command line. 

### How to use

*The functions `concert-this`, `spotify-this-song`, `movie-this`, and `do-what-it-says` will make an API call about your search string. The search strings does not need to be inside of quotes and can be multiple words. If you do not enter an artist, my default search will return to you information about my favorites.*

The `concert-this` function searches the Bands in Town Artist Events API, and returns the name of the artist you have searched and information about their next concert: the name of the venue, the city and country of the venue, and the date and time of that show.  

![](concertThisDieAntwoord.png)

![](concertThisDeadmau5Default.png)

The `spotify-this-song` function searches the Spotify API and returns information about the song in your terminal/bash window. Information returned is: artist(s), the song's name, a preview link of the song from Spotify, and the album that the song is from.

![](spotifyThisSongStrawberryWine.png)

![](SpotifyThisSongClairDeLuneDefault.png)

the `movie-this` function searches the OMDB API and the following information to your terminal/bash window: the movie title you searched for, the year it came out, the IMDB Rating of the movie, Rotten Tomatoes rating of the movie, the country where the movie was produced, the language of the movie, its plot, and actors in the movie.

![](movieThisSevenBridesForSevenBrothers.png)

![](movieThisWizardOfOzDefault.png)

The `do-what-it-says` function uses the fs Node package. With this, LIRI will take the text inside of random.txt and then use it to call LIRI's commands/functions. It should run spotify-this-song for "I Want it That Way," as it follows the text in random.txt. I will edit the text in random.txt to test out other functions.

![](DoWhatItSaysSpotifyThisSong.png)

![](DoWhatItSaysMovieThis.png)

## Github repository

(https://github.com/HannahSchuelke/liri-node-app)


## Built With

* [Node Spotify API](https://www.npmjs.com/package/node-spotify-api) - Spotify npm installed
* [Node Axios](https://www.npmjs.com/package/axios) - Axios package installed
* [OMDB API](http://www.omdbapi.com/) - Used to generate `movie-this` responses
* [Bands In Town API](http://www.artists.bandsintown.com/bandsintown-api) - Used to generate `concert-this` responses
* [dotenv](https://www.npmjs.com/package/dotenv) - Installed to load environment variables from my .env file into process.env

## Authors

* **Hannah Schuelke** - (https://github.com/HannahSchuelke)
