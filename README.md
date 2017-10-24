# react-tetris

> Embed a game of Tetris in your React app

```shell
$ npm install --save react-tetris
```

[view demo](http://brandly.github.io/react-tetris/)

```js
const React = require('react');
const Tetris = require('react-tetris');

const App = () =>
  <div>
    <h1>Tetris</h1>
    <Tetris>
      {({
        HeldPiece,
        Gameboard,
        PieceQueue,
        points,
        linesCleared
      }) => {
        return (
          <div>
            <div>
              <HeldPiece />
              <div>
                <p>Points: {points}</p>
                <p>Lines Cleared: {linesCleared}</p>
              </div>
            </div>

            <div>
              <Gameboard />
            </div>

            <div>
              <PieceQueue />
            </div>
          </div>
        )
      }}
    </Tetris>
  </div>
```

include some styles

```css
.game-block {
  margin: 0;
  padding: 0;
  width: 1.5em;
  height: 1.5em;
  border: 1px solid #ddd;
}
.piece-i {
  background-color: #ec858b;
}
.piece-j {
  background-color: #f1b598;
}
.piece-l {
  background-color: #f8efae;
}
.piece-o {
  background-color: #b5a677;
}
.piece-s {
  background-color: #816e56;
}
.piece-t {
  background-color: #b77c72;
}
.piece-z {
  background-color: #e3be58;
}
.piece-preview {
  background-color: #eee;
}
```
