# 1 : Write short notes on below array methods with code examples
# 1 - reverse()
- The built-in array reverse() method is the simplest way to reverse a string in JavaScript.
```js  
let arr = [1,2,3,4,5,6,7,8,9]
arr.reverse()
console.log(arr);     
```
# 2 - sort()
- The sort() method returns a reference to the original array, so mutating the returned array will mutate the original array as well. 

```js
let Fruits = ["banana", "apple", "jackFruit", "grapes"]
console.log(Fruits.sort());
```
# 3 - fill()
- The fill() method in JavaScript is used to fill all the elements of an array with a static value.

```js
let animals = ["Dog","cat","rat","Elephent"]
console.log(animals.fill("Dragon"));
```
# 4 - filtter
-The filter() method creates a new array filled with elements that pass a test provided by a function. 

```js
let arr = [10,15,20,45,65,30]
let outPut = arr.filter((item)=>{
return item >15
})
console.log(outPut);
```
# 5 - some
- The some() method of Array instances tests whether at least one element in the array passes the test implemented by the provided function. 

```js
let arr =[10,15,18,20,19]

let checking =arr.some((item)=>{
return item >20
})
console.log(checking);
```
# 6  - every
- The every() method executes a function for each array element. The every() method returns true if the function returns true for all elements. The every() method returns false if the function returns false for one element.

```js
let arr = [8,10,20,30,4,18]
let isEven=(num)=>{
return num%2===0
}
let result = arr.every(isEven)
console.log(result);
```
# 7 -map
- map() method is creates a new array from calling a function for every array element. map() does not execute the function for empty elements. map() does not change the original array.

```js 
let arr = [2,4,6,8,10,12,14,16,18,20,22]
let mul=arr.map((num)=>{
return num *2
})
console.log(mul);
```
# 8 - forEach()
- forEach() method is used to execute the function which is taken as a parameter and applied for each value in the set, in insertion order.

```js
let arr = [1,2,5,6,4,9]
let multiplication =arr.forEach((array)=>{
    console.log(array * 2);})
```
# 9 - reduce
- The reduce() method of Array instances executes a user-supplied "reducer" callback function on each element of the array, in order, passing in the return value from the calculation on the preceding element.

```js
let arr = [12,25,45,78,20,23,45]
let value=((total,num)=>{
return total+num
})
let result = arr.reduce(value)
console.log(result);    
```
# 10 - indexOf 
- The indexOf() method of String values searches this string and returns the index of the first occurrence of the specified substring.

```js
let arr = ["subin","bincy","subin"]
console.log(arr.indexOf("subin"));
```

# 2 : write a function that takes an array of numbers as an argument and returns the sum of its elements.
```js
let arr = [100,10,10,20,35]
let sum =((total,num)=>{
    return total + num
})
let result = arr.reduce(sum)
console.log(result);
```

# 3 : Create a function that filters strings in an array by their length
```js
let arr = ["mango","orange","apple","grap"]
let checking = arr.filter((array)=>
 array.length<5
)
console.log(checking);
```
# 4 : Create a function that returns a new array containing the square roots of each number in the original array [1,4,9,16,25](Math.sqrt())

```js
let arr = [1,4,9,16,25]
let newArray = arr.map((item)=>{
    return Math.sqrt(item)
})
console.log(newArray);
```
# 5.Write a function that prints the number 1 to 100. But for multiples of 3, print Fizz instead of the number, and for multiples of 5, print Buzz. For the numbers that are multiples of both 3 and 5, print FizzBuzz(write the code in the browser’s snippet and invoke the function inside the console)

```js
let  count = 1
let outPut = []
let counter = ()=>{
    if(count % 3 ===0 && count % 5 ===0){
        outPut.push("FizzBuzz")
    }else if(count % 3 ===0){
        outPut.push("Fizz")
    }else if(count % 5 ===0){
        outPut.push("Buzz")
    }else{
        outPut.push(count)
    }
    count++
     console.log(outPut)   
    }
    counter()
    
```