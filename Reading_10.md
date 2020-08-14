### Reading 10

####### Debugging

* When debugging your JS, always confirm that you have no syntax errors first. Your code will not run until those syntax errors are fixed.
* When hunting syntax errors, typically the actual problem is before the line that errored. Work backwards from there.
* Console.log everything! Often times the biggest errors come from faulty assumptions. That variable you thought was a string was actually an array of strings, which can completely 
  change your logic.
* Run your code early and often, especially at first. If you're writing 20 or 30 lines of JavaScript at a time before seeing if any of it works, you're coding too much! The stronger
  you get with JS, the more assumptions you can make, but at first assume nothing!
  
###### Key Rules of Hoisting
* Variable declarations (var) rise to the top of their scope like hot air balloons.

* Functions create their own scope and act like cages, preventing declarations from rising out.

* Assignments, or = signs, act like anchors. They stay put, no matter how the code is rearranged.

* let and const do not get hoisted,  and will throw an error if called before they are declared. const will even throw a syntax error if it is called before it is assigned.
