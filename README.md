# Data-Structures-and-Algorithms-LeetCode
In this repository i share the implementation of data structures and algorithms to most interviewed questions

#Explanation of least recent used cache

To implement a Least Recently Used (LRU) cache, you can use a doubly linked list and a hash map (dictionary). The doubly linked list stores the items in the order they were used, with the most recently used item at the front and the least recently used item at the end. The hash map stores the items with the keys as the keys and the address of the corresponding nodes in the doubly linked list as values.

When you add an item to the cache, you check if the cache is full. If it is full, you remove the last node in the doubly linked list and remove its entry from the hash map. If the cache is not full, you add the item to the front of the doubly linked list and add its entry to the hash map.

When you retrieve an item from the cache, you check if it exists in the hash map. If it exists, you move the corresponding node to the front of the doubly linked list and update its entry in the hash map. If it does not exist, you return an error or a default value.

This way, the least recently used item is always at the end of the doubly linked list and can be easily removed if the cache is full and a new item needs to be added.
