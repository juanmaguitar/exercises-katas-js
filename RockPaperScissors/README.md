# Kata: Rock Paper Scissors!

### Problem Description

We need a function `rockPaperScissors()` that can receive two parameters with the move of each of the two players in the game "Rock Paper Scissors".

The possible values are : "PAPER", "SCISSORS" or "ROCK"

If the function is called with only one parameter the move of the second player should be randomly generated.

```
>> rockPaperScissors("PAPER","SCISSORS")
"PAPER vs SCISSORS => SCISSORS wins!"

>> rockPaperScissors("ROCK","ROCK")
"ROCK vs ROCK => tie!"

>> rockPaperScissors("PAPER")
"PAPER vs ROCK => PAPER wins!"

>> rockPaperScissors("PAPER")
"PAPER vs PAPER => tie!"
```

### Stage 2 - new requirements

 Create an object called game with the following structure:

```
game = {
  player1: 0,
  player2: 0,
  rockPaperScissors : function() {...},
  winner: function() {...}
}
```

With this object created when we call the method `game.rockPaperScissors()` we store in `player1` or `player1` the number of games each player have won. When calling the method `game.winner()` we should receive a string telling which player is winning.

```
>>  game.rockPaperScissors("PAPER","SCISSORS")
"PAPER vs SCISSORS => SCISSORS wins!"

>> game.rockPaperScissors("ROCK","ROCK")
"ROCK vs ROCK => tie!"

>> game.rockPaperScissors("PAPER")
"PAPER vs ROCK => PAPER wins!"

>> game.rockPaperScissors("PAPER")
"PAPER vs PAPER => tie!"

>> game.rockPaperScissors("ROCK","SCISSORS")
"ROCK vs SCISSORS => ROCK wins!"

>> game.winner()
"player1 is winning!"
```