# D3 Chessboard ♕

A chessboard in D3. No CSS, no images, no (chess) validations, just a chessboard 
using the spirit of [reusable charts](http://bost.ocks.org/mike/chart/).

## How to use

1. Choose you selector!
2. Create the `d3chessboard()` element
3. Call it!

```
var sel = d3.select("#chess-container");
var board = d3chessboard();
sel.call(board);
```

![](images/screenshot_1.png)

## Options

You can use a FEN string to plot an specific position.
```
var fenstring = "rnbqkbnr/pp1ppppp/8/2p5/4P3/8/PPPP1PPP/RNBQKBNR w KQkq c6 0 2";
var sel2 = d3.select("#chess-container2")
var board2 = d3chessboard()
				.fen(fenstring)
				.width(450)
				.height(450)
				.whitecellcolor("#FAFAFA")
				.blackcellcolor("#CCC");

sel2.call(board2);
```
![](images/screenshot_2.png)

## Requirements

This plugin needs [jhlywa' chessjs](https://github.com/jhlywa/chess.js). Check `index.html`.

## References

1. http://bost.ocks.org/mike/chart/
2. https://github.com/jhlywa/chess.js
3. http://stackoverflow.com/questions/27806132/how-to-draw-a-chess-board-in-d3
