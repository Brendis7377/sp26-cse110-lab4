# part 2 - javascript questions 

## Question 1 : 
What will happen at line 12 and why? :
-**Answer:** Line 12 will print 13, this is because we declare i using var, which is in the scope of the function, so it can still be accessible even outside of the loop. After the loop finishes i will then have the value of 3, since the loop stops when i is equal to prices.length 

## Question 2 : 
What will happen at line 13 and why? :
-**Answer:** Line 13 will print 150, this is because we can see that discountedprice is declared using var, this means that it has a function scope and like the previois question can be accessed outside of the loop, the value will get updated everytime the loop runs as well as after the loop ends and it will keep the value from the last iteration. Because the last price is 300 and the discount is 0.5 then the final value will be 150 

## Question 3 : 
What will happen at line 14 and why? :
-**Answer:** Line 14 will print 150, this is because finalprice is also declared using var, meaning that it can acessed outside of the loop too making it function scope. Its value will be updated after each iteration of the loop occurs, after the loop finishes it will keep the value from the last iteration. Like the previous question the last price is 300 and the discount is 0.5 so then the final value will also be 150 

## Question 4 : 
What will this function return, give a brief explanation? : 
-**Answer:** The function will return [50, 100, 150], since it will loop through each of the prices in the array and then we also apply the 0.5 discount to each one. Then we can calculate the discounted values and add them into the discounted array which then we recieve back at the end of the function

## Question 5 : 
What will happen at line 12 and why? :
-**Answer:** Line 12 will now cause a reference error, this is because now we are using let, so i is being declared using let which is block scoped only and this means that it only exists inside of the for loop, because 12 is outside of the loop i wont be defined there 

## Question 6 : 
What will happen at line 13 and why? :
-**Answer:** Line 13 will also cause reference error, this is because discountedprice is now declared usinf "let" meaning that it is blocked scoped so it only exists inside of the for loop, line 13 is outside of the loop so it means that it will not be defined 

## Question 7 : 
What will happen at line 14 and why? : 
-**Answer:** Linr 14 will print 150, we know this because finalprice is declared outside of the loop so it will still be accessible evenn after the loop ends, the value updated after every iteration and the last value is kept which is 150.

## Question 8 : 
What will this function return? : 
-**Answer:** The function will return [50, 100, 150], this is because it will loop through each of the prices and add the doscount to each one, similar to the previous question. The results then are added to the discounted array which then will be returned at the end, there isnt any error since all the variables are used within the correct scope 

## Question 9 : 
What will happen at line 11 and why? : 
-**Answer:** Line 11 will cause a ReferenceError. this is because i is being now declared using let, so this means that it is block scoped which means that it only exists inside of the for loop. Since line 11 is outside the loop, then i is not defined

## Question 10 : 
What will happen at line 12 and why? : 
-**Answer:** Line 12 will print 3, this is because length is set to the length of prices array which we know is 3, because it is declared outside of the loop it will be accessible at line 12 

## Question 11 : 
What will this function return? : 
-**Answer:** The function will return [50, 100, 150]. this is because it will loop  through each price and then it applies the discount to each one. Then the discounted values are added to the discounted array, which is returned at the end. we see that there is no error because then all of the variables are used within their correct scope 


## Question 2

### A.
```js
student.name
student["Grad Year"]
student.greeting()
student["Favorite Teacher"].name
student.courseLoad[0]
```

## Basic Operators & Type Conversion 

### 3. Arithmetic
'3' + 2  
- Output: '32'  
- Explanation: The number 2 is converted to a string, so then it becomes string concatenation.

'3' - 2  
- Output: 1  
- Explanation: The string '3' is converted to a number, so then it will becomes 3 - 2 which is 1 .

3 + null  
- Output: 3  
- Explanation: null is then converted to 0, so it will become 3 + 0.

'3' + null  
- Output: '3null'  
- Explanation: null is converted to a string because '3', so it concatenates it doesnt turn to 0.

true + 3  
- Output: 4  
- Explanation: true is converted to 1, so it becomes 1 + 3 which is then 4.

false + null  
- Output: 0  
- Explanation: false becomes 0 and null becomes 0 so then 0 + 0 will equal 0 .

'3' + undefined  
- Output: '3undefined'  
- Explanation: undefined is converted to a string and then it is concatenated.

'3' - undefined  
- Output: NaN  
- Explanation: undefined cannot be converted to a number properly, so result is NaN.


### 4. Comparison

'2' > 1  
- Output: true  
- Explanation: '2' is converted to number 2, so 2 > 1 which is then resulting true.

'2' < '12'  
- Output: false  
- Explanation: Both of them are strings, so compared lexicographically ('2' > '1') not by the number itself.

2 == '2'  
- Output: true  
- Explanation: == means that it  does type conversion, so '2' becomes 2.

2 === '2'  
- Output: false  
- Explanation: === it will checks both the value and type, and they are different types so then it will result false.

true == 2  
- Output: false  
- Explanation: true will becomes 1, so 1 == 2 is false.

true === Boolean(2)  
- Output: true  
- Explanation: Boolean(2) is true, and === compares both type and value.


### 5. Difference between == and ===

The == operator will check if the values are equal after performing type conversion if needed. The === operator checks if both the value and the type are exactly the same, without actually converting the types

### 6. Is found in seperate part2-questions16.js 

### Question 7 : 
If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what will be the result? 
- **Answer:** The function will return [2, 4, 6] this is because the functun modifyArray will loop through each of the elements in the array [1, 2, 3] and then applies the doSomething function to each of the values, and the doSomething function will then multiply each of the numbers by 2, therefore the 1 will become a 2, the 2 will become a 4, and the 3 will become a 6. Then these values are added to the new array which is then returned at the en.