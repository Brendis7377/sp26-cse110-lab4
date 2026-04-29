# part 1 - javascript questions 

## Question 1 : 
What is printed by line 9? : 
- **Answer:** "values added: 20" , this is because of the sumValues(10, 10, true), since its true then it runs and the variable result holds num1 + num2, and then in line 9 we see console.log that outputs the number held in result plus the text "valudes added: " 

## Question 2 : 
What is printed by line 13? : 
- **Answer:** "values final result: 20" , it still remains 20 because the sumValues is called with add equaling to True, which means that the if block will run meaning that the else block wont ever run and so the value will remain as 20, this is because the function stores result as 0 then immediately updates it as num1 + num2 

## Question 3 : 
Why should you not use var? : 
- **Answer:** The keyword var is used to be able to declar variables in javascript as well as being accessible anywhere within a function even if it is declared in a specific code block like a conditional or if statement and we should not use it because it can cause bugs or unexpected behavior 

## Question 4 : 
What is printed by line 9? : 
- **Answer:** "values added: 20" , same as question 1, if sum values is true then the code will run true and the variables hold num1 + num2 is 10 and 10 so then the answer stored in result is 20 

## Question 5 : 
What is printed by line 13? : 
- **Answer:** error , it will result in an error because result is not clearly defined, this is different than last one since result is declared using let not var, which means result is only stored within the code block in the IF statement, so line 13 is out of scope 

## Question 6 : 
What is printed by line 9? : 
- **Answer:** A type error is printed because result is declared using const, which means that result can't be reassigned because const variables cant be reassigned which means its value cannot change, so when the line result = num1 + num2 tries to run there is an error 

## Question 7 : 
What is printed by line 13? : 
- **Answer:** A type occure will occur, this is the same as the previous question, because of result being declared with const, then line 13 cant ever update resulting in an error, but this error will occur before we even get to line 13 

## Question 8 is in part2-question18 

## Question 9 : 
What is the output of the above code? :
- **Answer:** the out will be from top to bottom 1 4 3 2 , this is because javascript runs asynchronously first meaning that 1 and 4 will be the first ones to print and then the function with the 0 delay will run before the one with the 1000 delay meaninf that 3 will run first and then 2 