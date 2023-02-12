
// var LRUCache = function (capacity) {: This line creates a constructor function for the LRUCache class.The constructor takes in a capacity argument, which specifies the maximum number of items the cache can store.

//     this.capacity = capacity;: This line sets the capacity property of the object created by the constructor to the capacity argument passed in.
    
//     this.map = new Map();: This line creates a new Map object and sets it to the map property of the object created by the constructor. The map will be used to store the key-value pairs in the cache.
    
//     this.head = { key: null, value: null, next: null, prev: null };: This line creates an object for the head of a doubly linked list, with properties for key, value, next, and prev. The linked list is used to keep track of the order of the items in the cache, where the least recently used item will be at the head and the most recently used item will be at the tail.
    
//     this.tail = { key: null, value: null, next: null, prev: null };: This line creates an object for the tail of the linked list, with the same properties as the head.
    
//     this.head.next = this.tail;: This line sets the next property of the head to the tail object.
    
//     this.tail.prev = this.head;: This line sets the prev property of the tail to the head object.
    
//     LRUCache.prototype.get = function(key) {: This line defines a get method on the LRUCache class. The method takes in a key argument and returns the value associated with the key. If the key is not in the cache, it returns -1.
    
//     if (this.map.has(key)) {: This line checks if the map has a key equal to the key argument.
    
//     let node = this.map.get(key);: If the key is in the map, this line retrieves the corresponding node from the map.
    
//     this.remove(node);: This line calls the remove method on the node retrieved in the previous step.
    
//     this.add(node);: This line calls the add method on the node retrieved in step 10.
    
//     return node.value;: This line returns the value of the node retrieved in step 10.
    
//     LRUCache.prototype.put = function(key, value) {: This line defines a put method on the LRUCache class. The method takes in a key and value argument and adds the key-value pair to the cache.
    
//     if (this.map.has(key)) {: This line checks if the map has a key equal to the key argument.