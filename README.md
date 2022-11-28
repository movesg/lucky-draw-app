# 🎉 Lucky Draw App
## 100% fair and transparent

A web app that collates every player and their number of chances and generates a list of all chances with a unique numeric Chance code. Winners are then picked using a random number generator.

Try out the app at luckydraw.streamlit.app

Example template downloadable [here](https://github.com/movesg/luckydraw/blob/main/example.xlsx)


### Background
Hidden Singapore is an immersive outdoor adventure game built by Move Technologies and led by our WhatsApp chatbot, Void Deck Cat. The game was featured during the Thomson East-Coast Line Phase 3 launch, organised by the Land Transport Authority. Each station had its own immersive game, and players earned points by playing and answering Void Deck Cat's quizzes correctly. Each point gave them a chance in the Grand Lucky Draw, which featured attractive prizes.

The LTA tasked us to run the lucky draw process and ensure that it is fair and transparent. Being the nerds we are, we decided to build a solution using Python.

### How It Works
At the end of the game, Void Deck Cat generates a spreadsheet of players and the total number of points / chances they've earned in the game - see [example](https://github.com/movesg/luckydraw/blob/main/example.xlsx)

This spreadsheet is uploaded onto the Lucky Draw App. The script iterates through every player and their number of chances, and generates a digital list of all chances and their serial numbers (in the form of CXXXXXX). Each chance is then assigned to a player according to the number of chances they have earned. 

### Example
Ali, Baoli, and Charlie played the game and earned chances as follows:

- Ali: 5 chances
- Baoli: 10 chances
- Charlie: 3 chances

The code generates a total of 18 chances, with serial numbers 1 - 18. Ali is assigned 5 of these chances, Baoli 10, and Charlie 3.

A spreadsheet of the list of chances and the players they are assigned to is made available for download via the app. 

### Selecting a winner
The Lucky Draw app includes a random number generator, using the _randint_ function, to generate a random number between 1 and the total number of chances. However, any random number generator can be used for this purpose. Google, for example, has one built into its search function, or there are other cool generators such as [Random.org](www.random.org) which uses atmospheric noise to generate randomness, instead of pseudo-random number algorithms typically used in computer programs. 

### Questions?
Drop us a line at hi@move.sg
