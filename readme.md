# Three.js Lottery Wheel

This is a simple lottery wheel using Three.js.

## Requirements

- [Three.js](http://mrdoob.github.com/three.js/)

## Usage

```
Lottery.init({
	digit: 4
});

Lottery.init({
    numbers: ['001', '128', '337', '751', '999'],
    actions: ['add', 'swap'],
    cubeSize: 300,
    cubeSpace: 50,
    cubesPerDigit: 5,
    waitingTime: 2000
});
```

### Options

Name            | Type    | Description                    | Default
------          | ----    | -----------                    | -------
`numbers`       | array   | manual lottery numbers         |
`digit`         | integer | automatic lottery numbers      |
`actions`       | array   | transition actions             | `['add', 'subtract', 'swap']`
`cubeSize`      | integer | width and height of a cube     | `200`
`cubeSpace`     | integer | space between each cubes       | `100`
`cubesPerDigit` | integer | cubes per each digit           | `10`
`waitingTime`   | integer | transition time (milliseconds) | `3000`

### Note

- Either `numbers` or `digit` must be set.
- `numbers` must be partial array of `['add', 'subtract', 'swap']`.
- It was tested in **Google Chrome** only. Not yet in other browsers. :(