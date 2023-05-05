Download Link: https://assignmentchef.com/product/solved-csf342-computer-architecture-lab-sheet-6
<br>
<strong style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;"><u>Goals for the Lab</u></strong><span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">: We build up on prior labs and explore basics of functions and recursion.</span>

<strong><u>Background</u></strong>:

<ul>

 <li>Calling a subroutine is between a <em>caller</em>, who makes the subroutine call, and the <em>callee,</em> which is the subroutine itself.</li>

 <li>The caller passes arguments to the callee by placing the values into the argument registers <strong>$a0-$a3.</strong></li>

 <li>The caller calls <strong>jal</strong> followed by the label of the subroutine. This saves the return address in <strong>$ra</strong>. The return address is PC + 4, where PC is the address of the jal instruction. If the callee uses a frame pointer, then it usually sets it to the stack pointer. The old frame pointer must be saved on the stack before this happens.</li>

 <li>The callee usually starts by pushing any registers it needs to save on the stack. If the callee calls a helper subroutine, then it must push $ra on the stack. It may need to push temporary <strong>($t0-$t7)</strong> or saved registers <strong>($s0-$s7)</strong> as well.</li>

 <li>Once the subroutine is complete, the return value is placed in <strong>$v0-$v1</strong>.The callee then calls <strong>jr $ra</strong> to return back to the caller.</li>

</ul>




<strong><u>Exercise 1 – With Sample Code</u></strong>: Study the code given below.







<strong> </strong>

<strong><u>Exercise 2</u></strong><u>:</u> Write a function to count the number of vowels in a given string and also return the string after removing the vowels and print that string in main function. Call the function twice with two different strings.




Input           : String (without space)




Output          : Single integer




<strong><u>Exercise 3</u></strong><u>:</u> Write a program that asks if the user wants a triangle or a square. It then asks the user for the size of the object (the number of lines it takes to draw the object). The program then writes a triangle or a square of stars “*” to the console.




*******

*******

*******

*******

*******

*******

or

*

**

***

****

***** ******

Write a subroutine for each figure. In them, use a subroutine <strong>print_star_line</strong> that writes a line of a given number of stars. (that number is passed as an argument to <strong>print_star_line</strong> function).




<strong><u>Take home assignment:</u></strong>

Print the pyramid as:

*

**

***

****

*****

******

*******







<strong><u>Exercise 4:</u></strong> Find Factorial of a given integer recursively<strong>. </strong>Take care of the base case.




<strong><u>Exercise 5:</u></strong> Disassemble the following hex instructions.

<ul>

 <li>02002009</li>

 <li>03e00008</li>

 <li>0c100013</li>

</ul>




<strong>References</strong>: <a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">http://stackoverflow.com/questions/18991655/how</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">–</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">do</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">–</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">you</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">–</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">perform</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">–</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">a</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">–</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">recursive</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">–</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">operation</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">–</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">in</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">mips</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">–</a><a href="https://stackoverflow.com/questions/18991655/how-do-you-perform-a-recursive-operation-in-mips-assembly">assembly</a>

<a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">http://stackoverflow.com/questions/22317560/mips</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">–</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">assembly</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">–</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">removing</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">–</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">vowels</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">–</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">from</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">–</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">an</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">input</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">–</a><a href="https://stackoverflow.com/questions/22317560/mips-assembly-removing-vowels-from-an-input-string">string</a>

<strong> </strong>