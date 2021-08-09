<!--nota javascrip-->
# Arrays pop(), push(), shift(), unshift(), splice,  slice.
---

### Pop()
*Using the keyword, pop, you can remove the last element of an array.
Suppose you have an array, pets, whose elements are "dog", "cat", and "bird". The
following code deletes the last element, "bird", leaving a two-element array.*
```JavaScript
pets.pop();
```
### Push

*using the keyword Push you can add one or more elemente at the end of the array*
```JavaScript 
/*orginal array */ pets = ["car", "perro", "roll"];
 pets.push("gato", "dog");
 /*after push */  pets = ["car", "perro", "roll", "gato", "dog"];
```
---
### shift() Arrays remove first element
 ```javaScript
 pets.shift();
 ```
 ---
 ### unshift Add more than one element at the begining of the array.
 ```javaScript 
 pets.unshift("fish", "ferret");
```
---
### Splice method array
#### Use the splice method to insert one or more elements anywhere in an array, while
*optionally removing one or more elements that come after it. Suppose you have an array with
the elements "dog", "cat", "fly", "bug", "ox". The following code adds "pig", "duck", and "emu"
after "cat" while removing "fly" and "bug".*
```JavaScript
pets.splice(2, 2, "pig", "duck", "emu");

```
*You could make additions without removing any elements. The following code adds
"pig", "duck", and "emu" without removing any elements.*
```JavaScript
pets.splice(2, 0, "pig", "duck", "emu");
```
*You can also remove elements without adding any. If you start with the elements "dog",
"cat", "fly", "bug", and "ox", the following code removes two elements starting at index 3
—"bug" and "ox". This leaves "dog", "cat", and "fly".*
```JavaScript
pets.splice(2, 2);
```
---
### Slice Method 
*Use the slice method to copy one or more consecutive elements in any position and put
them into a new array. If you start with an array, pets, consisting of "dog", "cat", "fly", "bug", and "ox", the following code copies "fly" and "bug" to the new array noPets and leaves the
original array, pets, unchanged.*
```JavaScript
var noPets = pets.slice(2, 4);
```
# For loop
```JavaScript
  
    var cleancity = ["nagua", "vega", "azua", "santo domingo", "santo domingo norte"];
    var numbercleancity1 = cleancity.length;
     var citytoCheck = "azua";
     var matchFound = false;
     for (var i = 0; i < numbercleancity1; i++) {
         if (citytoCheck === cleancity[i]) {
            matchFound = true;
             alert("congrat you are in the list")
             break;
         }
         
     }
      if (matchFound === false){
             alert("sorry bro")
    }
```
### replace a text with indexOF
#### we can also use lastIndexOf and segIndex
```JavaScript
var text = "Hola a todo hoy vamos hablar de World War II";
var textfinder = text.indexOf("World War II");
if (texfinder !== -1){
    text = text.slice(0, texfinder) + "the Second World war" + text.slice(textfinder + 12);
} 
```
### found a first and last character with charAt
```JavaScript
var name = "juan";
var firstchar = name.charAt(0);

var lastchar = name.charAt(name.length - 1);
```
### Found any character with ChartAt
```JavaScript
var text = "Dios es amor la biblia lo dice y punto!"
for (var i = 0; i < text.length; i++){
    if (text.chartAt(i) === "!"){
        alert("exclamation Found!")
        break;
    }else{
        alert("Not found")
        break;
    }
}
```
### replace method
```JavaScript
/*only one phrase*/
var text = "hola a todos";
var newtext = text.replace("hola", "hello");
/*global change */
var text = "hola a todos hola a todos";
var newtext = text.replace(/hola/g, "hello")
```
---
### random number
```JavaScript
var num1 = (Math.random() * 6) + 1;
var num2 = Math.round(num1);
```
### conver strings to integer and decimals
#### This example below convert the data entry by the user to interger
```JavaScript
/* Example parseInt and parseFloat*/
var currentAge = prompt("Enter your age.");
var convertoInt = parseInt(currentAge);

/* this example converte the string to interger round it string to 1 */
var myInterger = parseInt("1.999");

/*this example converte the string to number keeping the decimals*/
var myFloat = parseFloat("1.999")
```
### link event
#### this line below show an alert saying hi in a link. 
```JavaScript
<a href="JavaScript:void(0)" onClick="alert('Hi');">click me</a>
```