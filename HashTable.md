# Hash Table

<ol>
<li>Hash Table combines the random Access ability of the array with the dynamisim of the linked list.</li>
<li>So in hash table Insertion, Deletion and look up takes up only constant time which is <b>O(1)</b></li>
<li>Hash Tables over comes the disadvantages of using a linked list and an array.
  <ul>
    <li>Disadvantage of using a array - Specificing an constant size and when an array is dynamically resized its expensive.</li>
    <li>Disadvantage of using a linked list - It is harder to traverse/lookup a specific value in a linked list when the size of the linked list gets bigger.</li>
  </ul>
</li>
<li>In a hash table the data itself dictates or gies us clue on where the data is going to be stored and where we can find the data for easy look up. Eg.. A hash function would create would indicate where the valeu can be stored</li>
<li><i><b>Disadvantage of hash table :-</b><i>We should not use has table for sorting or ordering data. If used for sorting or ordering then insertion, deletion and lookup becomes close to <b>O(n)</b></li>
</ol>
