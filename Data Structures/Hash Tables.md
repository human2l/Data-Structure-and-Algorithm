# Hash Table

* key value pairs
* using hashing method to hash the key, allocate a memory based on the hashed key, save the key-value(both of them) to the memory

<img src="Hash Tables.assets/Screen Shot 2022-01-29 at 7.56.22 PM.png" alt="Screen Shot 2022-01-29 at 7.56.22 PM" style="zoom:25%;" />

O(n) lookup time in worst case (due to collision)

### Cons:

Get all the keys: `.key()` takes O(n) to loop through every memory cell to get all keys (even empty cell)

## Hash Collision

<img src="Hash Tables.assets/Screen Shot 2022-01-29 at 8.02.16 PM.png" alt="Screen Shot 2022-01-29 at 8.02.16 PM" style="zoom:50%;" />

When Hash Collision happens it slows down the process with O(n/k) => O(n). k is the size of hash table

## Map

In JS we can use `const a = new Map()`

Difference with JS Object: 

1. Map can use whatever data type as key
2. Map maintains insertion order, like Array, when we loop through Map, it has order

## Set

`const b = new Set()`

Set only store the key, no values

<img src="Hash Tables.assets/Screen Shot 2022-01-30 at 12.04.12 AM.png" alt="Screen Shot 2022-01-30 at 12.04.12 AM" style="zoom:25%;" />