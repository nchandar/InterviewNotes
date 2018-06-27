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

### Here's an example of a simple hash function
```javascript

function hashFunction(str) {
  var sum = 0, i;
  var strLength = str.length;
  for (i = 0; i < strLength; i++) {
    sum += str.charCodeAt(i); // charCodeAt(i) gets the ASCII value of the letter in i'th position
  }
  return sum % 10;  //10 is max size of the array in which the data is stored.
}

console.log(hashFunction("Paul"));
```
### Collisions
When the hashFunction returns the same hash code or key for 2 different values. Then collision is formed.
Collision can be avoided by using these 2 methods
<ul>
  <li><b>Linear Probing</b></li>
  <li><b>Chaining</b></li>
</ul>

#### Linear Probing
In this method if there is a collision, we try to place the data in the next position/element in the array.

![Image2](https://github.com/nchandar/InterviewNotes/blob/master/linearProbingFig.jpg) 

1. If you consider the above example using linear probing, you can already see that the constant time for inserting, deletion and lookup which is O(1) is now changing and in the worst case scenario it could O(n). This problem is called <b>clustering</b>.
2. We can only store data which equals the size of the array and so the data can never grow and it can only have n elements in the table where n is the size of the array.

#### Chaining
