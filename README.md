## More Problem solving

Remember:

* one step at a time (test thoroughly each step)
* researching a step is excellent (although time-consuming)

# 1
## Calculate the Cube
Write a function `calculateCube` that takes a single number and prints the volume of a cube made from that number.

```javascript
function calculateCube(num){
var Cube=num*num*num;
return Cube;
}

console.log(calculateCube(5));
```

> => 125


# 2
## Is a Vowel?
Write a function `isAVowel` that takes a character (i.e. a string of length 1)
and returns true if it is a vowel, false otherwise. The vowel could be upper or lower case.

```javascript
function isAVowel(letter){
letter=letter.toLowerCase();
if ((letter=='a')||(letter=='e')||(letter=='o')||(letter=='i')|| (letter=='u'))
  return true;

else
  return false;

}

console.log(isAVowel("A"));
console.log(isAVowel("u"));
console.log(isAVowel("g"));
```




# 3
## Get Two Lengths
Write a function `getTwoLengths` that accepts two parameters (strings). The function should return an _array_ of numbers where each number is the length of the corresponding string.

```javascript
function getTwoLengths(word1,word2){
var num1=(word1.split("").length )
var num2=(word2.split("").length )
var arr=[num1,num2];
return arr;
}

console.log(getTwoLengths("Hank", "Hippopopalous")); // [4, 13]
```

# 4
## Get Multiple Lengths

Write a function `getMultipleLengths` that accepts a single parameter as an argument: an **array of strings**. The function should return an array of **numbers** where each number is the length of the corresponding string.

```javascript
var num;
var arr2=[];
function getMultipleLengths(arr){
for(i=0;i<arr.length;i++){
num=arr[i].length;
arr2[i]=num;
}
return arr2 ;
}
console.log(getMultipleLengths(["hello", "what", "is", "up", "dude"])); // [5, 4, 2, 2, 4]
```



# 5
## Maximum of Three Numbers
Define a function `maxOfThree` that takes three numbers as arguments and returns the largest of them. If all numbers are the same, it doesn't matter which one is returned. If the two largest numbers are the same, one of them should be returned.

```javascript
function maxOfThree(n1,n2,n3){
if ((n1>n2)&&(n1>n3))
return n1;
if ((n2>n1)&&(n2>n3))
return n2;
if ((n3>n1)&&(n3>n2))
return n3;
if (n1=n3=n2)
return n1;
}

console.log(maxOfThree(6, 9, 1)); // 9
```

# 6
## Print Longest Word

Write a function `printLongestWord` that accepts a single argument, an **array of strings**. The method should return the longest word in the array. In case of a tie, the method should return the word that appears first in the array.


```javascript
var long=0;
var length=[];
var word='';
function printLongestWord (arr){
for (var i=0;i<arr.length;i++){
length[i]=arr[i].length;
if (length[i]>long){
    long=length[i];
    word=arr[i]
}
}
return word
}

console.log(printLongestWord(["BoJack", "Princess", "Diane", "a", "Max", "Peanutbutter", "big", "blob"])); //"Peanutbutter"
```


# 7
## Transmogrify the Numbers
Write a Javascript function called `transmogrify`. This function should accept three arguments, which you can assume will be numbers. Your function should return the "transmogrified" result.

The transmogrified result of three numbers is the product of the first two numbers, raised to the power of the third number.

For example, the transmogrified result of 5, 3, and 2 is `(5 times 3) to the
power of 2` is 225.



```javascript
function transmogrify(num1,num2,num3){
var result=Math.pow((num1*num2),num3);
return result;
}
console.log(transmogrify(5, 3, 2)); //225
```
