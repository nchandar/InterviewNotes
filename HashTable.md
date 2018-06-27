# Hash Table

<ol>
<li>Hash Table combines the random Access ability of the array with the dynamisim of the linked list.</li>
<li>So in hash table Insertion, Deletion and look up takes up only constant time which is <b>O(1)</b></li>
<li>Hash Tables over comes the disadvantages of using a linked list and an array.
  <ul>
    <li>Disadvantage of using a array - Specificing a constant size and when an array is dynamically resized its expensive.</li>
    <li>Disadvantage of using a linked list - It is harder to traverse/lookup a specific value in a linked list when the size of the linked list gets bigger.</li>
  </ul>
</li>
<li>In a hash table the data itself dictates or gives us a clue on where the data is going to be stored and where we can find the data for easy look up. Eg.. A hash function would create a key that would indicate where the value can be stored</li>
<li><i><b>Disadvantage of hash table :- </b></i>We should not use has table for sorting or ordering data.
<ul>
  <li>If used for sorting or ordering then insertion, deletion and lookup becomes close to <b>O(n)</b>.</li>
  <li>Never use the hash table if the data stored needs to sorted.</li>
</ul>
</li>
</ol>
<br/>

### How Hash Table Works
<ol>
<li>A Hashtable basically work with the combination of these two things..</li>
  <ol>
    <li><b><i>Hash Function :- </i></b>Returns a non-negative integer value call hash code.</li>
    <li><b><i>An Array :- </i></b>Which is capable of storing the data.</li>
  </ol>
<li>The idea is that we pass our data to the hash function and it returns a hash code. Then store the data into the array with the key represented by the hash code that was generated.</li>
</ol>

![ImageOne](https://github.com/nchandar/InterviewNotes/blob/master/HtFig1.jpg)
