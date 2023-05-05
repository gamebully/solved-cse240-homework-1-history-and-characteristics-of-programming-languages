Download Link: https://assignmentchef.com/product/solved-cse240-homework-1-history-and-characteristics-of-programming-languages
<br>
Introduction

The aim of this assignment is to make sure that you understand and are familiar with the concepts covered in the lectures, including Unix operating system, programming paradigms, the structure of programming languages, and the differences between a macro and a procedure. By the end of the assignment, you should have

<ul>

 <li>Learned a brief history of programming languages and the characteristics of the languages.</li>

 <li>Gotten started with Unix and GNU GCC the programming environment.</li>

</ul>

This assignment is related to the outcomes 1-2 and 1-3 listed in the syllabus:

<ul>

 <li>Students will understand the control structures of functional, logic, and imperative programming languages.</li>

 <li>Students will understand the execution of functional, logic, and imperative programming languages.</li>

</ul>

<strong>Reading</strong>:​ Read chapter 1, chapter 2 (sections 2.1, 2.2, and 2.3), appendix (sections B.1 and B.2), and course notes (slides).

You are expected to do the majority of the assignment outside the class meetings. Should you need assistance, or have questions about the assignment, please contact the instructor or the TA during their office hours.

Subscribe to the General UNIX Cluster Server. You need to visit the ASU Computer Accounts Self-Sub website: <u><a href="http://www.asu.edu/selfsub">http://www.asu.edu/selfsub</a></u>

You can login using your ASUAD User ID &amp; password. It will list your current subscriptions and what other options are available for you to subscribe. Add ASU <strong>General</strong>​ Computing Server if you don’t have it.

Your new General UNIX account may be ready immediately or may take a few days to become available. You can then log onto the “general.asu.edu” server using your ASUAD User ID and your password.

You need a secure telnet client like PuTTY or SSH to access the general server. You will use

ASU General account and PuTTY or SSH for C/C++ and Prolog programming in this course. You can also create your personal web page in the folder called www in ASU General server.

In this course, you will use GNU gcc compiler to run C programs. Later in the semester, you will be required to use GNU Prolog under the General server to run all your Prolog programs. The course is designed to give you experience of using different kinds of programming environments!

<ol start="2">

 <li>Getting Started with GNU GCC on Unix</li>

</ol>

To do the C assignments using GNU GCC, you need to have basic Unix knowledge. If you are not familiar with basic Unix commands, you need to read textbook Appendix B, sections B.1 and B.2.1 and the Unix Tutorial given in the homework folder.

For example, when I log in to ​<strong>General </strong>and perform a ​ ​<strong>pwd</strong>​ command, I see,

/afs/asu.edu/users/y/c/h/ychen1

Of course, it should be the path from the root to ​your directory​

<ul>

 <li>Do an ​<strong>ls</strong>​ command to see the files in your home directory.</li>

 <li>Do an ​<strong>ls -a</strong>​ command to see ​<strong>all </strong>​of the files in your home directory, including hidden files.</li>

 <li>Do an ​<strong>ls -l</strong> command to produce a ​ ​<strong>long </strong>​listing of the non-hidden files in your home directory.</li>

 <li>Do an ​<strong>ls -al</strong>​ command to produce a ​<strong>long </strong>​listing of <strong>all </strong>​​of the files in your home directory.</li>

</ul>

Make a new directory (e.g. MyDir or CSE240) by using the command: <em>mkdir</em>​<em> MyDir</em>​, use this to store all of your C and C++ programs in a specific directory. You may create subdirectories in this directory.

Enter the directory by using Change Directory command: <em>cd MyDir</em>​

Please note that you can remotely connect (using PuTTY or SSH) to the general server from anywhere, at any time, that is, you can do the assignment at home.

To write a GNU GCC program on a Unix server, you can either use a Unix editor, e.g., <em>vim</em>​ or <em>pico</em>​ or upload (using the same PuTTY software that includes SSH/telnet) a pre-edited file into your Unix directory <em>MyDir</em>​ ​. The name of a C program should have an extension .<em>c</em>​ and the name of a C++ program should have an extension .<em>cpp</em>​

<strong> </strong>Programming Exercise

<ol>

 <li>Follow the Textbook Appendix B and the Unix Tutorial PPT given in the homework folder to complete the following tasks:

  <ul>

   <li>Create a new directory called CSE240. Use cd CSE240 to enter the new directory. Use pwd command to find the path from the Unix root directory to your current directory.</li>

   <li>Create three new subdirectories inside CSE240. Name the directories d1, d2, and d3 respectively.</li>

   <li>Enter the directory d1 and use vi or vim to create a new program called hello.c and enter the following code into the program. You must use your name ​ to replace the name “​ John​ Doe”. Save the file.​</li>

  </ul></li>

</ol>




Use <em>gcc hello.c -o hello</em>​ ​ to compile the program. Fix any compilation errors if any.

<ul>

 <li>Use ls, ls -l, and ls -al respectively to list files in d1 directory. [4 points] Use command ./hello to execute the compiled code.</li>

</ul>

Take screenshots of each command in this question. You may take one screenshot with all commands in it.

<ul>

 <li>Enter d2 directory and then use one command to copy (not move) the files hello.c and hello from d1 directory into d2 directory. Use ls -al to view all the files in d2.</li>

</ul>

Take screenshots of each command in this question. You may take one screenshot with all commands in it.        [3 points]

<ul>

 <li>In d2 directory, use chmod 660 hello to change the permission. Use ls -l to view the files. Use command ./hello to execute the compiled code. Take a screenshot of this output. Use chmod command again to make hello an executable, but not readable and not</li>

</ul>

writeable for all users. Use command ./hello to execute the compiled code. Take a

screenshot of this output.                                                                                           [4 points]

<ul>

 <li>Enter CSE240 directory. Use ls -l to view all the files. Then, use one command to delete d2 directory and all the files in d2 directory. Use ls -l to view all the files.</li>

</ul>

Take screenshots of each command in this question. You may take one screenshot with all commands in it.        [3 points]

Screenshots needed for questions 1.4 through 1.7. Put all the screenshots along with their question numbers in a word file and convert to pdf. Submit the file as hw01q1.pdf

<ol start="2">

 <li>In this question, you will use Unix tools to edit, debug, and execute a simple C program. The purpose of the homework is to learn the Unix programming environment. Read textbook Section 2.2.3, the tutorials, and the Unix tutorial in text Appendix B.2.

  <ul>

   <li>Use a text editor to enter the program on textbook page 47 (the code is given here for your convenience). Use GNU GCC to compile, debug (find and fix any syntax errors), and execute the program and fix any semantic errors, for example, by adding “break” statements in the required places and by fixing incorrect characters copied into the programming environment, if any, and by type-changing to print a floating point number. The code is supposed to perform one math operation in each switch-case. The ‘ch’ variable is assigned a new math operator before each switch-case. Submit the corrected program as hw01q2.c [8 points]</li>

  </ul></li>

</ol>




<table width="0">

 <tbody>

  <tr>

   <td rowspan="3" width="7"> </td>

   <td colspan="3" width="529">/* This C program demonstrates the switch statement without using breaks. */</td>

   <td rowspan="3" width="51"> </td>

  </tr>

  <tr>

   <td colspan="3" width="529">#include​ ​&lt;stdio.h&gt; int ​main() {char​ ch = ​’+’​; int​ a = 10, b = 20;        double f; printf(​”ch = %c
”​, ch); switch​ (ch) { case ​ ‘+’​ :​ f = a + b; printf(“f = %d
”​ , f);​ case​ ​’-‘:​ f = a – b; printf(“f = %d
”​ , f);​ case​ ​’*’​: f = a * b; printf(“f = %d
”​ , f);​ case​ ​’/’​: f = a / b; printf(​”f = %d
”, f);​ default​: printf(​”invalid operator
”​);} ch = ​’-‘​;printf(“ch = %c
”​ , ch);​ switch​ (ch) { case​ ​’+’:​ f = a + b; printf(“f = %d
”​ , f);​ case​ ​’-‘:​ f = a – b; printf(​”f = %d
”​, f); case​ ​’*’​: f = a * b; printf(“f = %d
”​ , f);​ case​ ​’/’​: f = a / b; printf(​”f = %d
”​, f); default​: printf(​”invalid operator
”​);} ch = ​’*’;​printf(​”ch = %c
”​, ch); switch​ (ch) {</td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td width="299">case ‘+’: f = a + b; printf(“f = %d
”, f);</td>

   <td width="182"> </td>

  </tr>

  <tr>

   <td width="7"></td>

   <td width="48"></td>

   <td width="299"></td>

   <td width="182"></td>

   <td width="51"></td>

  </tr>

 </tbody>

</table>

​​​ ​ ​

<table width="0">

 <tbody>

  <tr>

   <td rowspan="2" width="55">   ​return}</td>

   <td width="299">case​ ​’-‘​: f = a – b; printf(​”f = %d
”​, f);</td>

   <td rowspan="2" width="233">           </td>

  </tr>

  <tr>

   <td width="299">case​ ​’*’​: f = a * b; printf(​”f = %d
”​, f); case​ ​’/’​: f = a / b; printf(“f = %d
”​ , f);​ default​: printf(​”invalid operator
”​);} ch = ​’/’;​printf(​”ch = %c
”​, ch); switch​ (ch) { case​ ​’+’​: f = a + b; printf(“f = %d
”​ , f);​ case​ ​’-‘​: f = a – b; printf(​”f = %d
”​, f); case​ ​’*’​: f = a * b; printf(“f = %d
”​ , f);​ case​ ​’/’​: f = a / b; printf(​”f = %d
”​, f); default​: printf(​”invalid operator
”​);} ch = ​’%’​;printf(​”ch = %c
”​, ch); switch​ (ch) { case​ ​’+’​: f = a + b; printf(“f = %d
”​ ​, f); case​ ‘-‘​ :​ f = a – b; printf(“f = %d
”​ , f);​ case​ ​’*’​: f = a * b; printf(“f = %d
”​ , f);​ case​ ​’/’​: f = a / b; printf(​”f = %d
”​, f); default​: printf(​”invalid operator
”​);}​ 0;</td>

  </tr>

 </tbody>

</table>




<ul>

 <li>Edit the code above or write a new code to use a for-loop (that runs 5 times) to ask the user for a math operation as input ( +, – , * , / ). Use an input statement such as <em>ch</em>​<em> = getchar();</em> or <em>scanf(“%c
”,</em>​<em> &amp;ch);</em> to replace the assignment statement <em>ch</em>​<em> = </em>​<em>‘+’ </em>​in the code above. Expected result shown in figure below. Submit the revised program as hw01q2_2.c.             [8 points]</li>

</ul>




Note, you may need to use a <em>fflush(stdin)</em>​ or a <em>getchar();</em>​ to flush the newline character left behind by a previous operation <em>getchar()</em>​ ​;.

<ol start="3">

 <li>You are given a file named “hw01q3.c”. All instructions are given in the form of comments in the file. You should correct the errors and identify which error type they are. Please read all instructions carefully, then complete and submit the updated file. [20 points]</li>

</ol>

<h1>What to Submit?​</h1>

This homework assignment will have multiple parts. You are required to submit your solutions in a compressed format (.zip). Make sure your compressed file is labelled correctly – lastname_firstname1.zip.   (All lowercase, do not put anything else in the name like “hw1”.)

The compressed file MUST contain the following:




hw01q1.pdf            (screenshots from questions 1.4 through 1.7)

hw01q2_1.c     (program) hw01q2_2.c             (program) hw01q3answer.c (program)




No other files should be in the compressed folder.

If multiple submissions are made, the most recent submission will be graded. (Even if the assignment is submitted late.)




Submission preparation notice: The assignment consists of multiple files. You must copy these files into a single folder for blackboard submission. To make sure that you have all the files included in the zip file and they work after unzip operation, you must test them before submission. You must also download your own submission from the blackboard. Unzip the file on a different machine, and test your assignment and see if you can open and test the files in a different location, because the TA will test your application on a different machine. If you submitted an empty project folder, an incomplete project folder, or a wrong folder, you cannot




resubmit after the submission linked is closed! We grade only what you submitted in the blackboard. We cannot grade the assignment on your computer or any other storage, even if the modification date indicated that the files were created before the submission due dates. The blackboard submission may take a few minutes. Be patient and wait for it to complete.





