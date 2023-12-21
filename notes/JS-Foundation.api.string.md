---
id: bs95q9944wj2vturdnz0v1m
title: String Methods
desc: ""
updated: 1702882621505
created: 1702882522404
---

#### Length of String

```js
str_name.length;
```

#### Find Index Of

```js
string.indexOf(target); // finds index of first occurrence of target in string
string.lastIndexOf(target); // gives index of last occurence of target
```

#### Slice

```js
"sample_string".slice(0,4)
: samp

slice(start,end) // from start till end excluding end index
```

#### Replace

```js
str.replace("to_replace", "replacer");
```

#### Split

```js
Example:

const str = "Hi I am Rohan"
const words= str.split(" ");
// splits string based on telemeter("" here) to an array
 words: ['Hi','I', 'am','Rohan']
```

#### Trim

```javascript
str.trim("  Helllllo     ");

str: Helllllo;
// Trims the extra space in the beginning and at the end of the string
```

#### Case

```javascript
str1.toUpperCase("rohan");

// str1: ROHAN

str2.toLowerCase("SHARMA");

//str2: sharma
```
