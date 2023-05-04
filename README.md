Download Link: https://assignmentchef.com/product/solved-csci1300-1310-assignment-9-code-in-python-using-known-programming-constructs
<br>



<ol>

 <li>Design and create code in python using known programming constructs</li>

</ol>




For this assignment, you will be submitting your code to Moodle code runner. In this assignment you will be converting your assignment 3 which was in C++ to python(Python 3).

Read the entire assignment carefully before beginning. In this assignment, you’re going to develop a simulated community message board where users can post items they have for sale or search for items they want to buy. Your program will search for matches, e.g. there is a bicycle for sale for $50 and a bicycle wanted, where the buyer will pay up to $60, and remove items from the message board as they are sold. Users have the option of posting and searching for as many items as they choose before they quit the program.




<strong>Getting</strong> ​ <strong>started</strong>​                                                                                                               <strong>        </strong>

Your program should display a menu with the following selections:

<ol>

 <li>Insert an item.</li>

 <li>Search for an item.</li>

 <li>Print the message board.</li>

 <li></li>

</ol>




Use the following python print statements for your menu:




print “1. Insert an item.”  print “2. Search an item.” print “3. Print the message board.”  print “4. Quit.”




The input is going to be passed from a file so a suggested input line is




choice = myFile.readline()

//before the menu loop you need to open myFile with a parameter filename,

//which you read from input before the  –i.e. filename = input()







This menu should be displayed after every transaction is complete unless the user selects Quit. The user can select the option they want using the number for the option. For example, to add an item, they type 1.




<strong>Insert</strong>If the user ​ <strong>an</strong>​ ​ <strong>item</strong>​ selects  1 to add an item, they should be prompted for the type of item to add and the cost of the item. To simplify the program, there are five types of items: bicycle, microwave, dresser, truck and chicken. Your input prompts need to include the exact text shown here:




“Enter the item type-b,m,d,t,c:”

“Enter the item cost:”




The user types the first letter of the item type to indicate the type they want to add. Data in the message board is stored as a list of lists. Each element on the message board is a list that contains the type and the cost, and all of the individual elements are stored in the message board list.




Your list will look something like this:




[[‘bicycle’, 50], [‘truck’, 1000], [‘microwave’, 10]]




In this example, there are three elements in the message board list, a bicycle for $50, a truck for $1000, and a microwave for $10. The first element in the message board list is a list with two elements: the string “bicycle” and the integer 50, which is the cost. Each of the individual lists in the message board has two properties, a string and an integer.




When an element is added to the message board list, it should be appended to the end of the list. Don’t sort the data, Duplicates are also okay.




<strong>Search for</strong> ​ <strong>an</strong>​ ​ <strong>item</strong>​ selects  2 to search an item, they should be prompted with the item When the user

type, and the maximum price they are willing to pay for the item. Your code should then search the list and return the first item with the correct type and a cost that is less than or equal to the price that the user will pay.




Use the following text in your prompts:




“Enter the item type-b,m,d,t,c:” “Enter the maximum item cost:”




For example, if the user types b and 50, they want a bicycle and are willing to pay up to $50 for it. Your program should find the first bicycle in the list that sells for $50 or less.




If a match is found, print “Sold &lt;type&gt; for &lt;cost&gt;”




The <em>itemType</em>​ .​  is one of the following: <strong>bicycle,</strong>​ ​<strong>microwave,</strong> <strong>dresser,</strong>​ <strong>truck,</strong>​ or <strong>chicken</strong>




The <em>itemCost</em>​ ​ is the actual item cost, not what the user is willing to pay.

The item should then be removed from the list.

If the item is not found, do nothing.




<strong>Print</strong> ​ <strong>the</strong>​ <sub>user</sub> ​ <strong>message</strong>​ selects <sub>Print</sub> ​ <strong>board</strong>​<sub> the</sub> <sub> </sub>message board, your program should display the items in <sub>If</sub> <sub>the </sub>the message board list in the following format:




&lt;type&gt;: &lt;cost&gt;




<strong>Quit </strong>

If the user selects 4 for Quit, the program should exit the while loop that controls the program, which will cause the program to exit.




<strong>Format</strong> ​ <sub>be</sub><strong>and</strong>​<sub> submitting</sub> ​ <strong>ordering</strong>​                                        ​<sub>your</sub><strong>of</strong>​ ​ <strong>program</strong>​<sub> assignment</sub> ​          <strong>output</strong>​ to <sub>the</sub> <sub> </sub>moodle, so it’s important that the output

<sub>You</sub> will

of your program is formatted and ordered in a certain way. You should use the print

Don’tstatements given in this write output anything other​- up.<sub>than</sub> <sub> </sub>what is specified. Even the seemingly harmless newline character or space could spell doom.