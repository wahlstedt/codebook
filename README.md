# Codebook
A simple-to-use tool to generate pages you print out to play a fun cooperative wordgame.

## How to use
- Download the html file either with git or use the [zip link](https://github.com/wahlstedt/codebook/archive/refs/heads/master.zip).
- Open the html file in a browser, either your local copy or the one [online](http://wahlstedt.github.io/codebook/). 
- Drag a textfile with words onto the page. Use one of the included wordlists or your own.
- Adjust the options to set the style and number of games to generate.
- Print the pages from your browser, or save them as a pdf.
- Play the game with friends!

## Game rules
This plays pretty much like [Codenames Duet](https://czechgames.com/files/rules/codenames-duet-rules-en.pdf) so if you know how to play that you are good to go. The main difference is that you play with pen and paper instead of cards and tokens.

It is a cooperative wordgame for two or more players where the game gives you words to give single-word clues for and words your partner must avoid.

A clue is only one word, but it can point to multiple words that you want your partner to select. You and your partner 
take turns giving clues and selecting words. If you find all the words before you run out of turns, you both win.

Each player has their own page with the same selection of words, but mixed up differently. The large section on top is 
the list of all the words and is the same for both players. The smaller list below with the double outline contains 
the target words you want your partner to select. The list below that, with the single outline, are words you want 
your partner to avoid. Finally, the black words at the bottom are words that your partner absolutely must not select because if that happens, you both lose the game!
       
### Setup
A game consists of 2 pages. Each player takes one of the pages, A or B. Make sure they have the same id. 

The top list of words is identical to both players, but the smaller lists below are different and should not be revealed to your partner.

Choose a starting player, then alternate turns giving clues.
### Turns
You give a clue by saying a single word and a number. The number tells how many words relate to the clue.

Your partner then selects a word he thinks your clue refers to and says it out loud.

If the word is in your list of target words you say it was a correct word and your partner can continue selecting more words, or opt to end the turn.

If the word is among your black words, you both lose the game.

Otherwise, the selected word is incorrect and the turn ends immediately.

### Using the papers
At the start of a round you note down the word and number for the clue in the tracker.

When a *correct* word is selected you circle it **both** in the upper and lower lists.

When an *incorrect* word is selected you cross it off in only one list; the upper one if you are the guesser, the 
lower ones if you are the clue giver.

When a *black* word is selected you tear the paper up and start a new game...

After a turn ends you note down how many words were found and if any words remain, to keep track of progress.  

### Tracker table
Each row is a turn and the columns are:
1. Player giving the clue (e.g. A/B or initials).
2. Clue word.
3. Clue number.
4. Correct words. The number of words found this turn.
5. Incorrect words. Put a 1 if an incorrect word is selected.
6. Remaining words. The number of words left to find from this clue.
      
### Rule details
#### Clues
Your clue must be about the meaning of the words. You can't use your clue to talk about the letters in a word or its position in the list.

You can't use any part or form of an unfound word as a clue.

Clue givers can't give any indication about whether a correct guess was the word they were thinking of for their clue, and must refrain from any comments or reactions that could assist the guesser.

It is legal to assign 0 for clue number. But your partner must still select at least one word.
                 
#### Out of words
If all of your target words have been found, you notify your partner, who will now be the one giving clues on all 
remaining turns.

#### Sudden death
If players run out of turns they enter sudden death mode. No more clues can be given nor strategy discussed. Players make guesses in any order, one at a time, in an effort to find all words. Any mistake ends the game with a loss.

#### Word mixing
The table at the top of the page shows you how the words are mixed between the two players. Use this knowledge to your advantage. For example, 3 of your 9 target words are also target words for your partner. This overlap is why you only need to find 15 words in total.

Of your 3 black words, one is also black for your partner. Another is a target word and one is unused. 
This means that one of your black words is a word you must select. Furthermore, if you have found the black word 
that is a target word on the other side, you should not select any of the other two black words.
   
#### Scoring
Scoring is optional, but can be used to compare games with others.

+2 points per target found, +10 per unused turn, -5 per mistake, -10 if sudden death.
Games ended by a black word score differently: -10 points for each unused turn, mistake, and unfound target word.

## Settings
Most settings should be fairly self-explanatory, the advanced ones might require some explanation:

### Game variants
The standard game has 25 words, where each player has 9 target words and 3 black words, and you both need to find a total of 15 words in order to win.
By using the advanced 
settings you can create new variants by changing the number of words and their distribution.

You do this by editing the numbers in the table of word combinations. There's 3 different word types: target words 
(stars), unused words (empty circle) and black words (black circle). These can be combined in 9 ways, but since the 
game is symmetric (both players have the same combinations) you can only adjust 6 values.

The values for the combinations where the words are the same type for both players are set _in total_, while the other
combinations are set with the number _per player_, in order to keep the game symmetric.
   
### Interactive mode
The _first_ page is by default interactive to enable play on device. Click on words to toggle their status. Found 
words are automatically marked in both sections.

Click on the tracker table cells to enter clues or toggle values.

## Troubleshooting
### Printing
Chrome is recommended and known to produce correct pages. Safari seems to have issues with printing and can split up pages in weird ways.

## Acknowledgements
Inspired by [cnpaperplay](https://github.com/dcmouser/cnpaperplay) which in turn is based on the boardgame 
[Codenames Duet](https://czechgames.com/en/codenames-duet/).
