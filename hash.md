# Hash Tables

Hash Table also further improves on the Linked List. Hash Table is a higher level data structure: it uses other data structures to form another data structure. Hash table uses an array that will act as specific keys to put in new objects. Every time an object wants to be inserted or searched, it first goes through a hashing function which will determine its location in the Array. By using a Hash Table we can cut down a super long Linked List into smaller Linked List. With a hashing function, we would know to go to which Linked List to find the particular value or insert a particular value. If we had an Array of 26 possible spots, we can technically break down a single Linked List into 26 smaller ones. Our goal should be to find a hashing function that will normalize the long Linked List out evenly across the available spots in the Array.

Step 1: Implement the simpleHash, simplePut function

Step 2: Implement linkPut which will create arrays for each key to deal with collisions

Step 3: Implement a betterHash function that will result in a more widely distributed hash table

```
functioncopy HashTable() {
  // given fixed size of array of 26 slots
  this.table = new Array(26);
}
HashTable.prototype.buildLinks = function() {
  // set an empty array for all indexes in this.table
}
HashTable.prototype.linkBuilt = function() {
  // determines if links have been built yet
}
HashTable.prototype.simpleHash = function(data) {
  // determines the hash value given data
  // how can we use the ASCII values to find appropriate data (use charCodeAt())
}
HashTable.prototype.betterHash = function(data) {
  // how can we write a better Hash using ASCII values?
}
HashTable.prototype.simplePut = function(data) {
  // place data in appropriate place by using simpleHash
}
HashTable.prototype.linkPut = function(data) {
  // build links if not built yet and place data in the right place
}
HashTable.prototype.showDistribution = function() {
  // shows distribution of hash table
  for(var i = 0; i < this.table.length; i++) {      
    console.log(this.table[i]);    
  }
}
var names = ["Tony", "Tori", "Kate", "Kyle", "Thomas", "Dale",
             "David", "Daisy", "Andy", "Albert", "Dane", "Shane", "Lane",
             "Janet", "Katelyn", "Janet", "Vivian", "Joe"];
var simpleHashTable = new HashTable();
for(var i = 0; i < names.length; i++) {
  simpleHashTable.simplePut(names[i]);
}
simpleHashTable.showDistribution();
var betterHashTable = new HashTable();
for(var i = 0; i < names.length; i++) {
  betterHashTable.linkPut(names[i]);
}
betterHashTable.showDistribution();
```
