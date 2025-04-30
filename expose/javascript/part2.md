1. Line 12 will print 2 since we increment our i for each iteration and are able to use this variable outside of the block.
2. Line 13 will print 150 since it will be the last iteration (last item) of the discounted price from the price array.
3. Line 14 will print 150. It is similar to the previous question but the Math.round is applied
4. The function will return 50,100,150, we proceed through the function and the result is a discounted array of the prices.
5. Line 12 will produce an error, because i is block scoped and not accessible outside of the block.
6. Line 13 will produce an error since we use the let keyword for discountedPrice, the block scoped variable may not be accessed outside the for loop.
7. Line 14 is going to print out 150 because even though we use the let keyword, we initialize finalPrice it in the function and not only within the for loop.
8. The function returns 50,100,150. We proceed as normal. Throughout each loop we apply the discount on each price in the prices array and return the discounted array.
9. Line 11 will cause an error because we have used the let keyword inside the for loop when initialiazing i, so trying to use it outside of the block is invalid.
10. Line 12 will print 3. We use the const keyword to have our length be saved to 3 and then we are able to use this throughout the rest of the function.
11. The function will proceed as usual, even though discounted may use the const keyword, this does not mean the array is immutable so we will see the function proceed as usual and output 50,100,150.
12.a student.name;
12.b student['Grad Year'];
12.c student.greeting();
12.d student['Favorite Teacher']['name'];
12.e student.courseLoad[0];
13.a '32', JS converts 2 into a string and concatenates them.
13.b 1 since JS always uses '-' as numeric, so 3 becomes a number and subtracts 2.
13.c 3 because null is treated as a 0 for arithemtic operations in JS
13.d Because one of the operands are a string, JS treats null as a string so we have '3null'
13.e True is converted to a 1 and we add 3, so we have 4.
13.f In JS, false becomes a 0 and null is also a 0 for arithmetic operations so the sum is 0.
13.g '3undefined' since the '+' operator treats undefined as a string for concatenation.
13.h NaN, since the '-' operator requires numeric operands and attempting to convert undefined into a number will result in NaN.
14a. True, '2' will be converted into the number and evaluate the inequality.
14b. True, comparing two strings will be done through lexicographic means and '2' comes before '12'
14c. True, the == operator will perform type conversion automatically. This converts '2' to 2 and then makes the comparison
14d. False, the === operator is the strict equality operator and checks value and type. Because '2' is a string and 2 is a number, the output is false.
14e. True, because of type conersion true will be convereted to 1 and compares 1 and 2 whichi s false.
14f. True, Boolean(2) becomes true since all non-zero numbers are true, with === it checks that both value sand types which results in true.
15. The differece is that == compares values after converting their types. On the other hand, === compares value and type without conversions.
16. /Users/nkchang/sp25-cse110-lab4/expose/javascript/part2-question16.js
17. When we call modifyArray with the given array, we first create a new separate array and for each number in the original array [1,2,3], we use callBack, which in this case is the function doSomething(num), so for each number we multiply it by 2. In the end we have an array that is [2,4,6].
18. /Users/nkchang/sp25-cse110-lab4/expose/javascript/part2-question18.js
19. The code should output :
20. 1
4
3
2
console.log(1) executes immediately and logs 1, then 2 will only be logged after 1 second. The logging of 3 will happen after console.log(4) , setting the timeout for 0 will run after current call stack is cleared.