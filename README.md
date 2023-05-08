Download Link: https://assignmentchef.com/product/solved-python-program-that-plays-a-guess-the-number-game-with-magic-lists
<br>
Write a Python program that plays a guess-the-number game with magic lists.

The program will play as many games as the user wants. In each game, the program asks the user to think of a number between 1 and 31, inclusive. Then the program presents the user with 5 lists and asks the user if their number is in the list. Based on the user’s answers of ‘y’ or ‘n’, the program guesses the user’s number.

<ul>

 <li>The program works with 5 files, each file contains 16 integers, one number per line.</li>

</ul>

The filenames are: magicList1.txt, magicList2.txt, magicList3.txt, magicList4.txt, and magicList5.txt

<ul>

 <li>The program is divided into 3 functions.</li>

</ul>

1. A createList function that will read in data from one magicList file.The function does the following tasks:

<ul>

 <li>

  <ul>

   <li>Create an empty list.</li>

   <li>Use the with construct to open the file magicListN.txt, where N is the input argument for the function.</li>

   <li>Loop to read in each line in the file, convert the line to an integer, and store the integer in the list.</li>

  </ul></li>

 <li>Return the list.</li>

 <li>Note: don’t call any list variable with the name “list”. “list” is a Python data type and is a reserved word. Some common ways to call a generic list variable are: List or _list or list_ or L , if you don’t want to use the more descriptive name magicList.</li>

</ul>

2. A checkList function that will check whether the user number is in the magic list.The function does the following tasks:

<ul>

 <li>Use a nested loop to print the magic list (16 numbers) as a table of 4 rows and 4 columns.</li>

 <li>Loop to ask the user if their number is in the list, stop the loop when the user answers ‘y’ or ‘n’The condition for the loop must be whether the user answers ‘y’ or ‘n’</li>

</ul>

3. A main function that will:

<ul>

 <li>Loop to create an <em>outer list</em> of magic lists. The loop will:

  <ul>

   <li>run 5 times to call createList, and each time store the returned magic list into the <em>outer list</em>.</li>

  </ul></li>

 <li>Loop to let the user keep playing as long as the user wants:

  <ul>

   <li>Create an inner loop that runs 5 times:

    <ul>

     <li>Call checkList to ask the user whether their number is in a particular magic list, passing to checkList one magic list at a time. Recall that the magic lists are elements in the <em>outer list</em> that you created in the step above.</li>

     <li>If the user answer is ‘y’ and:

      <ul>

       <li>it’s magicList1, then add 16 to the total</li>

       <li>it’s magicList2, then add 8 to the total</li>

       <li>it’s magicList3, then add 4 to the total</li>

       <li>it’s magicList4, then add 2 to the total</li>

       <li>it’s magicList5, then add 1 to the total</li>

      </ul></li>

    </ul></li>

   <li>Ask the user if they want to continue, and loop back to play again if the answer is ‘y’</li>

  </ul></li>

 <li>When done, if the total is non-zero, then print the user’s numberIf the total is 0, then print an error message</li>

 <li>Don’t forget to call the main function so that the program will run.</li>

</ul>

C. (10 pts) Test your output by running several games, one after another.