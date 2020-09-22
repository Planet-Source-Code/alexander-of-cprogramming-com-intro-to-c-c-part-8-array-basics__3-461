<div align="center">

## Intro to C/C\+\+ Part 8: Array Basics


</div>

### Description

This is the eight installment of my lessons, and it is on arrays. Arrays are essentially a way to store many values under the same name. You can make an array out of any data-type, including structures.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Alexander of CProgramming\.com](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/alexander-of-cprogramming-com.md)
**Level**          |Intermediate
**User Rating**    |4.3 (13 globes from 3 users)
**Compatibility**  |C\+\+ \(general\)
**Category**       |[Data Structures](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/data-structures__3-8.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/alexander-of-cprogramming-com-intro-to-c-c-part-8-array-basics__3-461/archive/master.zip)





### Source Code


<p><font face="Verdana">For example, you could say <br>
<br>
int examplearray[100]; //This declares an array</font></p>
<p><font face="Verdana">This would make an integer array with 100 slots, or
places to store values. The only difficult thing is that it starts off with the
first index-number, that is, the number that you put in the brackets to access a
certain element, is zero, not one!</font></p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; Think about arrays like this:
[][][][][][] Each of the slots is a slot in the array, and you can put
information into each one of them. It is like a group of variables side by side
almost.</font></p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; What can you do with this
simple knowledge? Lets say you want to store a string, since C++ has no built-in
datatype for strings, in DOS, you can make an array of characters.</font></p>
<p><font face="Verdana">For example:</font></p>
<p><font face="Verdana">char astring[100];</font></p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; Will allow you to declare a
char array of 100 elements, or slots. Then you could get it from the user, and
if the user types in a long string, it will all go in the array. The neat thing
is that it is very easy to work with strings in this way, and there is even a
header file called STRING.H. I will have a lesson in the future on the functions
in string.h, but for now, lets concentrate on arrays.&nbsp; The most useful
aspect of arrays is multidimensional arrays.</font></p>
<p><font face="Verdana">For example:</font></p>
<p><font face="Verdana">int twodimensionalarray[8][8];</font></p>
<p><font face="Verdana">Think about multidimensional arrays:</font></p>
<p><font face="Verdana">[][][][][]</font></p>
<p><font face="Verdana">[][][][][]</font></p>
<p><font face="Verdana">[][][][][]</font></p>
<p><font face="Verdana">[][][][][]</font></p>
<p><font face="Verdana">[][][][][]</font></p>
<p><font face="Verdana">This is a graphic of what a two-dimensional array looks
like when I visualize it.</font></p>
<p>&nbsp;</p>
<p><font face="Verdana">declares an array that has two dimensions. Think of it
as a chessboard. You can easily use this to store information about some kind of
game, or write something like tic-tac-toe. To access it, all you need are two
variables, one that goes in the first slot, one that goes in the slot. You can
even make a three dimensional array, though you probably won't need to. In fact,
you could make a four-hundred dimensional array. It is just is very confusing to
visualize.</font></p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; Now, arrays are basically
treated like any other variable. You can modify one value in it by&nbsp;putting:</font></p>
<p><font face="Verdana">arrayname[arrayindexnumber]=whatever;</font></p>
<p><font face="Verdana">You will find lots of useful things to do with arrays,
from store information about certain things under one name, to making games like
tic-tac-toe. One little tip I have is that you use for loops to access arrays.
It is easy:</font></p>
<p><font face="Verdana">#include &lt;iostream.h&gt;</font></p>
<p><font face="Verdana">void main()</font></p>
<p><font face="Verdana">{<br>
int x, y, anarray[8][8];//declares an array like a chessboard<br>
for(x=0; x&lt;8; x++)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">for(y=0; y&lt;8; y++)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">anarray[x][y]=0;//sets all members to zero once loops is
done</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">for(x=0; x&lt;8;x++)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">for(y=0; y&lt;8; y++)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">cout&lt;&lt;&quot;anarray[&quot;&lt;&lt;x&lt;&lt;&quot;][&quot;&lt;&lt;y&lt;&lt;&quot;]=&quot;&lt;&lt;anarray[x][y]&lt;&lt;&quot;
&quot;;//you'll see</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">Here you see that the loops work well because they
increment the variable for you, and you only need to increment by one. It is
simple, and you access the entire array, would you want to use while loops?</font></p>

