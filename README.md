# Problem Set 3.2.1
## Structured Problem Solving

### 1. 1000 Lights
You have a bank of switches before you, numbered from 1 to `n`. Every switch is connected to exactly one light that is initially off. You walk down the row of switches and toggle every one of them. You walk back to the beginning of the row and start another pass. On this second pass, you toggle switches 2, 4, 6, and so on. On the third pass, you go back to the beginning again, this time toggling switches 3, 6, 9, and so on. You continue to repeat this process until you have gone through n repetitions.

Write a program that takes one argument — the total number of switches — and returns an array of the lights that are on after `n` repetitions.

**Examples:**
```javascript
function lightsOn(switches) {
  // ...
}

lightsOn(5);        // [1, 4]
// Detailed result of each round for `5` lights
// Round 1: all lights are on
// Round 2: lights 2 and 4 are now off;     1, 3, and 5 are on
// Round 3: lights 2, 3, and 4 are now off; 1 and 5 are on
// Round 4: lights 2 and 3 are now off;     1, 4, and 5 are on
// Round 5: lights 2, 3, and 5 are now off; 1 and 4 are on

lightsOn(50);       // [1, 4, 9, 16, 25, 36, 49]
lightsOn(100);      // [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
```

### 2. Diamonds
Write a function that displays a four-pointed diamond in an nxn grid, where n is an odd integer supplied as an argument to the function. You may assume that the argument will always be an odd integer.

**Examples:**
```javascript
diamond(1);
// logs
*
```

```javascript
diamond(3);
// logs
 *
***
 *
 ```

```javascript
diamond(9);
// logs
    *
   ***
  *****
 *******
*********
 *******
  *****
   ***
    *
```

### 3. Now I Know My ABCs
A collection of spelling blocks has two letters per block, as shown in this list:

```
B:O   X:K   D:Q   C:P   N:A
G:T   R:E   F:S   J:W   H:U
V:I   L:Y   Z:M
```

This limits the words you can spell with the blocks to only those words that do not use both letters from any given block. You can also only use each block once.

Write a function that takes a word string as an argument, and returns `true` if the word can be spelled using the set of blocks, or `false` otherwise. You can consider the letters to be case-insensitive when you apply the rules.

**Examples:**
```javascript
isBlockWord('BATCH');      // true
isBlockWord('BUTCH');      // false
isBlockWord('jest');       // true
isBlockWord('Carmen');     // false
isBlockWord('Marcy');      // true
```

## 
<sup>Exercises adapted from [Launch School](https://launchschool.com)</sup>
