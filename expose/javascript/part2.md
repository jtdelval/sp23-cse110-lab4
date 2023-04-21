1. The console will output "3"-- we loop 3 times incrementing i afterwards. Because i was declared with "var", we can access it outside of the block.
2. The console will output "150"-- because discountedPrice was declared with "var" we can access it outside of the block, and the last iteration of the loop has discountedPrice = 300 * (1-.5) = 150
3. The console will output "150"-- because finalPrice was declared in this scope, and at the last iteration of the loop, we have finalprice = Math.round(discountedPrice * 100)/100 = discountedPrice = 150
4. The function will return [50,100,150]. The function applies the 50% discount to all prices and returns the updated list of new prices.
5. The code causes an error: i was declared with "let" but is accessed outside of its scope.
6. The code causes an error: discountedPrice was declared with "let" but is accessed outside of its scope.
7. The console will output "150"-- finalPrice was declared in this scope, and at the last iteration of the loop, we have finalprice = 150, so that is its most recent value.
8. This function will return [50,100,150]. The function applies the 50% discount to all prices and returns the update list of new prices.
9. The code causes an error: i was declared with "let" but is accessed outside of its scope.
10. The console will output "3"-- lengthw as declared in this scope, and remains unchanged.
11. This function will return [50,100,150]. The function applies the 50% discount to all prices and returns the update list of new prices.

12:

A: student.name;

B: student['Grad Year'];

C: student.greeting();

D: student['Favorite Teacher'].name;

E: student.courseLoad[0];

13:

A: '32'. Because the first element is a string, and + can represent string concatenation, it concatenates '3' and '2'

B: 1. Although the first element is a string, - is an arithmetic operator, so we peform 3-2=1.

C: 3. Given a number and an arithmetic operation, null is transformed into zero, and 3+0=3

D: '3null'. Because '3' + is perceived as string concatenation, null is transformed into the string 'null'.

E: 4

F: 0. Boolean and a + becomes an arithmetic sum, with "false" and "null" both being treated as zero.

G: '3undefined'. '3' + is perceived as string concatentation, so undefined is transformed into 'undefined'.

H: NaN. - is an arithmetic operator, so '3' is transformed into 3. With this, undefined is transformed into the number NaN (not a number), which when subtracted from 3 turns the whole thing into NaN.

14:

A: true. transformed to numbers, 2 > 1 is true

B: false. Compared as strings, '2' has a greater value than '1', so '2'<'12' is false. 

C: true.  2=='2' is true==true

D: false. these are two separate values.

E: false. this transforms to 1==2, which is false.

F: true. Boolean(2) transforms that side into true, so the whole statement is true===true which is true.

15: == will convert the types of the items being compared, === will not.

16: See part2-question16.js

17: [2,4,6]. We call the function modifyArray with arguments array=[1,2,3] and callback=doSomething, which doubles whatever its input is. In modifyArray, we first create newArr, after which we push each element of array into newArr after applying callback (after doubling it). This means we push 2, 4, and then 6. After this we return newArr.

18: See part2-question18.js

19: 1 4 3 2. 1 and 4 execute immediately, 3 executes during the next event cycle, 2 executes after a second delay