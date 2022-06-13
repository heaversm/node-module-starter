# Barebones Node Setup

This is a very simple node.js repo that allows you to run code samples. I'm using it to solve code examples from advent of code 2021, and it was taken from [Christiana Man]((https://github.com/mancristiana/advent-of-code-2021)(thank you for sharing). To run a specific code sample, first `npm i` in the root, then change to the folder where the javascript file resides (e.g. `cd/src/01`) and `node [filename].js`.

The code samples include a helper function (`utils/readinput.js`) which just loads a textfile with data.

```
const inputPath = fileURLToPath(new URL('./input.txt', import.meta.url))
const data = await readInput(inputPath)
data.split('\n').map((i) => Number(i))
```
