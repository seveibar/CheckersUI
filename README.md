# Checkers UI Library

This is a simple library for using creating a checkers board in a browser

![Example Checkers Board](https://raw.githubusercontent.com/seveibar/CheckersUI/master/exampleboard.png)

## Usage

See the index.html for an example.

### Initialize

```javascript
CheckersUI.init("#myCheckersBoardCanvas", {
  width: 500,
  height: 500
});
```

### Validate

```javascript
CheckersUI.validate = function(board){
  // validate board
  return true; // move is acceptable
}
```

### Getting the board

```javascript
CheckersUI.getBoard()
```

Returns the board as a 32 integer array where...
-2 = King of black
-1 = Piece of black
0 = no piece
1 = Piece of red
2 = King of red

### Load a custom board

```javascript
CheckersUI.load(board);
```
