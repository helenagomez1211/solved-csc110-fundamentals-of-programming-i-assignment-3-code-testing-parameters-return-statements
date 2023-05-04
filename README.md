Download Link: https://assignmentchef.com/product/solved-csc110-fundamentals-of-programming-i-assignment-3-code-testing-parameters-return-statements
<br>
<strong>Learning outcomes </strong>

When you have completed this assignment, you should understand:

<ul>

 <li>How to write <em>tests </em>to ensure that code runs as intended.</li>

 <li>How to write and call a <em>static method</em> that receives <em>parameters</em>.</li>

 <li>How to <em>return</em> a value from a <em>static method</em>.</li>

 <li>How to use <em>String methods</em>.</li>

 <li>How to <em>indent and document</em> a Java program.</li>

</ul>







Download and update the Java program named <em>Encode.java</em>. The program includes a method named <em>encrypt</em> that accepts a String and an int as parameters. The method will return a new encoded String by adding the integer value to each character’s ASCII value, as shown in the examples and following algorithm below.

<strong> </strong>

<strong><u>Examples:</u> </strong>

<strong>1)</strong><strong> String:  </strong><strong>HELLO  key: </strong><strong>2       </strong>                        2)  <strong>String:  TEST       key: 11 </strong>

H + 2 = J                       T + 11 = E

E + 2 = G                       E + 11 = P

L + 2 = N                       S + 11 = D

L + 2 = N                       T + 11 = E

O + 2 = Q




Resulting String: JGNNQ          Resulting String: EPDE




<strong><u>Note:</u></strong>  T + 6 would result in Z. Adding 11 to T went past the value of Z, with 5 remaining. In this case the remaining 5 are counted beginning at the start of the alphabet, resulting in E.




<strong><u>Algorithm:</u> </strong>

String <strong>message</strong>, int <strong>key</strong> are passed in as parameters. 1. Create a new empty String <strong>encodedMessage</strong>

<ol start="2">

 <li>Convert the String to upper-case.</li>

 <li>For each character in <strong>message</strong>

  <ol>

   <li>Convert each character to its integer value</li>

   <li>Assign this value to an int <strong>characterValue </strong></li>

   <li>Add <strong>key</strong> to <strong>characterValue</strong>. Make sure the new value is within the acceptable range**</li>

   <li>Convert <strong>characterValue</strong> back to a character and add it to the end of <strong>encodedMessage</strong></li>

  </ol></li>

 <li>Return <strong>encodedMessage</strong></li>

</ol>




** Work on getting the encrypt method working for simple examples first (like example 1 above) before working on more difficult examples (like example 2, where the letters wraps around from Z back to the start of the alphabet)




In your program, you will fill in the code for 3 methods

<ol>

 <li>A static method called <em>testing()</em>, which does the following:

  <ol>

   <li>Creates a String to be used as the message to be encoded.</li>

   <li>Creates an int to be used as the encryption key for the encoding.</li>

   <li>Creates another String to hold the result of the encoding.</li>

   <li>Tests the <em>encode</em> method with multiple messages and encryption keys</li>

  </ol></li>

</ol>




Note: The example on the previous page shows that the message: HELLO with key: 2 results in the encoded message: JGNNQ. You must test that this is true in your solution. Another recommended follow-up test might be to make sure that the message: JGNNQ with key: -2 results in the encoded message:  HELLO. The encrypt method must be completed before these tests will work.




<ol start="2">

 <li>A static method called <em>encrypt()</em>, which does the following:

  <ol>

   <li>Follows the algorithm outlined in the previous page to encode a message given a String and int passed in as parameters.</li>

   <li>Returns the encoded message.</li>

  </ol></li>

</ol>




<ol start="3">

 <li>A static method named <em>userInteraction()</em>, which does the following:

  <ol>

   <li>Creates and uses a Scanner and its <em>nextLine()</em> and <em>nextInt()</em> methods to read input from the user to get values for the message and key.</li>

   <li>Further tests the encrypt method using these values.</li>

  </ol></li>

</ol>




Advice: Build this method in parts, compiling and running after each major addition to your code to check that the code does work as you expect. For example, you might first create the String and int variables in the <em>testing()</em> method and then work on the <em>encrypt()</em> method and initially test its implementation with simple values (don’t worry about wrapping around Z right away). After that, write further tests in your <em>testing()</em> method and figure out the complicated cases in your <em>encrypt()</em> method.

<strong><em> </em></strong>

<h1>File to submit: Encode.java</h1>

<strong> </strong>

<strong><u>Marking</u>  </strong>

Your mark will be based on the following criteria:

<ul>

 <li>Your code <em>must compile and run</em>. It must prompt the user, read text input, and produce the expected output as described and shown above.</li>

 <li>Your code must conform to the requirements mentioned above (i.e., have <em>testing(), encrypt()</em> and<em> userInteraction()</em></li>

 <li>Your code must follow the guidelines outlined in Style_Guidelines.pdf, found through the Lectures &amp; Stuff link in the Lab Resources folder on connex.</li>

</ul>