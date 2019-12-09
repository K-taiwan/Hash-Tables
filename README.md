# Hash-Tables

What are hash tables and why should you care?

Hash tables help solve the problem with retrieving data in very large data sets. Essentially what happens is a hashing algorithm will turn an input into an output and store this information as needed. Important note... the algorithm must always get that same output. 

Lets use finding a word in the dictionary as an example of using a hash table. Normally you would need to search through the dictionary one by one to find the word. With a hashing algorithm of using the length of each word you could put them into a table. 
Enter collisions. The problem with adding your words in at a certain number (in this case the length of the word) is that there are many words with length 4, 5, and 6. To solve this what a hash table will do is have a bucket of sorts that can store multiple values.

For instance, the words "four", "none", and "dice" all have length four and would be in the four length bucket.

What the hashing algorithm would also be able to do is find that a certain word is in a particular bucket. This helps effectively skip the line so that the developer can get to the correct bucket and search there.


A hash function takes in a key(string/integer) for a data record(key-value pair) and returns an integer memory address, or an index in a table where that record can be stored. In other words, it maps some key from the very large universe of possible keys to a much smaller range of possible indices in a hash table.

Also when a hash function returns the same value for two different keys, this will call a collision.

Linear probing helps remove collisiosn by changing one index to the right until there is an open idex which can store the key without causing collision.

In addition another method would be chaining, this involves each table to contain "bucket", which can hold more than one record. These "buckets" are data structures that can be inserted as many key's/record's into them. This will make sure no collisions occur. The performance factor is faster, but much more memory is needed.
