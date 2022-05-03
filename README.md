# Garbage

## Description of this python code and what it does

### This python file will run a variation of Garbage, a simple children’s card game also sometimes called trash. The first step is to learn how to play Garbage, which is most easily accomplished by watching this tutorial video: https://www.youtube.com/watch?v=tKWvR-43Ukc

As the video describes, game play is quite simple. Each player is dealt 10 cards from a standard 52 card
deck,  which  are  placed  face  down  in  front  of  the  player  in  two r ows,  conceptually  labeled  1  through  10
(we’ll call this 10-card configuration the player’s table). The remaining cards are placed in a draw pile.

The game is played in rounds: w ithin a round, players alternate taking turns. A t urn begins with the player
drawing a card (typically from the draw p ile but optionally from the discard pile). If the position on the
player’s t able  whose  label  corresponds  to  the  draw v alue  is  face  down,  it  is  replaced  with  by  the  draw
(face  up),  and  the  replaced  card  is  then  compared  to  the  player’s t able.  Thus  begins  a  series  of
replacements,  which  only  ends  when  (i)  the  card  in  play  is  does  not  correspond  to  a  labeled  position  on
the table, or (ii) the card in play corresponds to a labeled position with a face up card. At this point, the
card in play is added, face up, to the discard pile and the turn ends.

The round proceeds turn-by-turn until one player manages to fill their table with cards placed face up in
label order. At t his point, the round is finished, and the losing player(s) are awarded the sum of the labels
of  the  face-down  cards  that  remain  on  their  table:  note  that  the  player  who  completed  his  or  her  table
earns  0  points,  which  implies  that  the  player  with  the  lowest  point  total  at  the  end  of  the  game  is  the
winner (indeed, this is the case).

The game proceeds round-by-round, but after each round the winning player’s t able size is reduced by 1
face-down for all subsequent rounds. The game ends when any p layer table is reduced to zero size.

First,  Trash  is  entirely  a  game  of  luck;  the  player  makes  essentially  no  choices  while  playing  the  game!
Drawing  a  card  starts  a  chain  of  replacements  until  nothing  more  can  be  replaced.  The  only  choice  a
player makes is whether to draw h is or her card from the draw p ile or the discard pile. But even t his is a
false choice: if the card from the discard pile matches a face-down card on the player’s t able, the correct
choice is to draw f rom the discard pile: so this is hardly a choice.

Second,  the  number  of  players  and  the  size  of  the  initial  table  can  be  parameterized  with  only  minimal
concern.  Indeed,  it’s p erfectly  reasonable  to  play  Trash  with  one  player  as  a  solitaire!  It’s a lso  perfectly
reasonable  to  play  with  more  than  two p layers.  The  only  concerns  are  (i)  that  the  length  of  the  game
measured  in  rounds  will  increase  with  the  number  of  players  and  the  initial  table  size,  and  (ii)  as  the
number of players grows, so must the size of the deck. To s ee why t he latter is so, consider that if there
are more than four players with a standard deck, there is a good chance that the game will not terminate,
since  no  player  is  guaranteed  that  they w ill  be  able  to  collect  all  of  the  cards  required  to  complete  their
table.




Next You should download the repository to your local computer and open up the .py folder on your favorite IDE. THe read through all the 
function explanations. After that, go ahead and test out the game of garbage!
