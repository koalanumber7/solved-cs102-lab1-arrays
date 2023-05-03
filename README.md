Download Link: https://assignmentchef.com/product/solved-cs102-lab1-arrays
<br>
Notes:

<ul>

 <li>For all labs in CS 102, your solutions must conform to these <a href="http://www.cs.bilkent.edu.tr/~adayanik/cs101/practicalwork/styleguidelines.htm">CS101/102 styl</a>​ <a href="http://www.cs.bilkent.edu.tr/~adayanik/cs101/practicalwork/styleguidelines.htm">e</a> <a href="http://www.cs.bilkent.edu.tr/~adayanik/cs101/practicalwork/styleguidelines.htm">guidelines</a>.​</li>

 <li>Create a Java Project named Lab01. Put all of your classes in this project.</li>

 <li>Remember to include <strong>javadoc</strong>​ ​ <strong>comments</strong>​     for each class and method.​</li>

 <li>Upload your solution <strong>as a single .zip file</strong>​ to the Lab01 assignment for your section​       by the end of your section’s lab session on the week of February 8. You must use the following naming convention: Lab01_Surname_FirstName.zip where Surname is your family name and FirstName is your first name. You may upload multiple times; the last upload will be considered.</li>

</ul>

<strong>Question </strong>In​ this lab, you are going to implement2 an <strong>Polynomial</strong>​ class that​ represents polynomials of the form P(x) = c​0 + c​1x + c​2x​ <sup>​</sup> + … + c​nx​

​               ​                  ​                                   ​

The class should do the following:

<ol>

 <li>Polynomial class should contain its coefficients in an array. Use double type for​</li>

 <li>Include a constructor that takes an integer, d​ , and a double, ​ c​ , to construct​ polynomials of the form P(x) = cx​           ​<sup>d</sup><sup>​</sup>.</li>

</ol>

Include a default constructor that takes no argument and constructs a zero polynomial (P(x) = 0​ ).​

<ol start="3">

 <li>Include another constructor that takes an array of coefficients and produces a polynomial with these coefficients.</li>

 <li>Add a getter method for a coefficient which takes degree and returns the coefficient of the term with that degree.</li>

 <li>Include <strong>getDegree()</strong>​ method that returns the degree of the polynomial. Degree of a​         polynomial is the degree of highest non-zero term in a polynomial. For example, the degree of polynomial P(x) = 4 – 5x​ ​<sup>2</sup><sup>​</sup> + 12x​<sup>3</sup><sup>​</sup> is 3. You can assume that the degree of zero polynomial is 0.</li>

 <li>Add <strong>toString()</strong>​ ​ method that returns ​  String​              representation of the polynomial.​        Zero terms in the polynomial should not be included in the string.</li>

</ol>

For instance, for the polynomial P(x)​ = 4 – 5x​<sup>2</sup> + 2x​<sup>3</sup><sup>​</sup>, toString()​ method should return “4.0 – 5.0x^2 + 2.0x^3”​         .​

<ol start="7">

 <li>Add <strong>eval( double x )</strong>​ method that evaluates the polynomial at ​       x ​          and returns​        the result.

  <ol>

   <li>Use pow( double a, double b )​ method to evaluate each term​ individually and the polynomial as a sum of the terms.</li>

   <li>Implement another method, <strong>eval2( double x )</strong>​ that evaluates the​ polynomial using Horner’s method. Horner’s method is an efficient way of evaluating polynomials at a given point. A polynomial P(x) = c​              ​0 + c<sub>​    </sub>​1x +<sub>​        </sub> c​2x<sub>​ </sub><sup>2</sup>​ <sup>​</sup> + … + c​nx<sub>​ </sub><sup>n</sup>​ <sup>​</sup> can be evaluated at x​ ​0 by rearranging computation as<sub>​   </sub></li>

  </ol></li>

</ol>

P(x​0)​ = (( … ( (c​n)​ x​0 + c​ n-1​​) x​0 … + c​ 4​ ) x​ ​0​ + c ​3)​ x​0 + c​ ​1)​ x​0 + c​ ​0 and​ computing the result from the innermost parentheses to outwards.

<ol start="8">

 <li>Implement a class called <strong>PolynomialTester</strong>​ to test your ​     Polynomial​  ​</li>

</ol>