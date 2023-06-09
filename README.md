Download Link: https://assignmentchef.com/product/solved-comp1410-lab-6-character-arrays-and-strings
<br>
,.’rn to use and manipulate strings and arrays of characters.

In C, a string is simply defined as an array of characters terminated by the null character, or string delimiter, ‘ ’.  If we want to store a string “hello”, which has only 5 characters, we need an array of minimum size 6. For example the array S below that has been declared as char S[6].  The array index (or subscript) values are indicated above each box containing a single character in the figure below.

We can also create a pointer to S: char *ptrS = S.  Then, if we apply pointer arithmetic and increment the pointer ptrS++ we can show that the pointer ptrS now points to the second item in the array with index 1 (refer to the figure below). Now we can refer to the letter ‘e’ by either using the pointer as *ptrS, or using the array index as S[1].

<strong>Lab Work to do: </strong>

Write a complete C language program called Lab6.c.  The requirements and specifications for the program are listed below in Parts A-C.  Read the entire set of lab instructions carefully before proceeding in order to appreciate and understand how to approach the design of your program.  Apply both Top-Down and Bottom-Up aspects of design.

Your program must treat each Part separately, but it is not required to have a menu, nor to loop back to receive multiple inputs – just do what is asked of you!

<strong>Part A. Character array and string. </strong>

<ol>

 <li>Declare a char array called buffer1 and initialize it to “this is the first buffer.” using</li>

</ol>

this method: {‘t’, ‘h’, ‘i’, ‘s’, ‘ ‘, ‘i’, … ‘ ’};

<ol start="2">

 <li>Declare a char array called buffer2 and initialize it to “this is the second buffer.” using this method: “this is the second buffer”;</li>

 <li>Declare a char array called buffer3 of size 80 and leave it un-initialized.</li>

 <li>Use the scanf function to initialize buffer3 from the keyboard. (Note: use %s as the formatting character for string). If you encounter problems, document them and work out solutions for them.</li>

 <li>Now, use printf to print all the three buffers. (Again, use %s as the formatting character for string data).</li>

 <li>Declare a pointer variable named pBuffer and initialize it to point to buffer3. (Use char * pBuffer).</li>

 <li>Display the contents of buffer3 using pBuffer; do not use subscripts.</li>

 <li>Advance the pointer pBuffer a few positions and display the rest of buffer3 (i.e.</li>

</ol>

only from that position to the end of the string) using pBuffer.

<strong>Part B.  String Manipulation: Reverse. </strong>

<ol>

 <li>Write a function called Reverse that accepts as a parameter a char array (or char pointer) and returns a void type. The function reverses the contents of the array (or string) being passed. Example: the string “Hello” will be reversed to “olleH”. You have to be careful about the ‘ ’ symbol to keep it at the end of the array and watch out for odd and even length of strings.</li>

 <li>Test your function and display the string (array) before and after it is reversed.</li>

 <li>IMPORTANT: The function does NOT print the string in reverse; it actually reverses it in the memory.</li>

</ol>

<strong>Part C. String Tokenization </strong>

<ol>

 <li>Write a function called ParseSentence that takes as input parameter a null (i.e. ‘ ’) terminated string S, where S would contain an English sentence./</li>

 <li>Assume that the delimiters are space, comma, semicolon and period.</li>

 <li>The function extracts each word from the sentence (without any punctuation or spacing) and then prints one word per line.</li>

 <li>The function returns a void type.</li>

</ol>

For example: <strong>char str[] = “hello world, how are you today.”; </strong>

<strong>ParseSentence(str); </strong>would print the following: <strong>hello world how </strong>

<strong>are you </strong>

<strong>today</strong>