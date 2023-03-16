This is repo for task 1-basic python, please clone this repo and create your own branch then push your work to this.
In this task, please create a readmne file then working on it and push to your branch


Data Type:
+ Text: str (String)
+ Numeric: int (Integer), float, complex ( 4j → always come with j)
+ Sequence: list, tuple, range
+ Mapping: dict
+ Set: set, frozenset
+ Boolean: bool
+ Binary: bytes, bytearray, memoryview
+ None: NoneType

#####################################################################
#####################################################################

Condition and Looping:
+ Equals: a == b
+ Not Equals: a != b
+ Less than: a < b
+ Less than or equal to: a <= b
+ Greater than: a > b
+ Greater than or equal to: a >= b

If condition: 
a = 33
b = 100 
if a < b
	print(True)

Elif condition: if the previous conditions were not true, then try this condition
Else: catch anything which is't caught by the preceding conditions.
And: logical operator, and is used to combine conditional statement **
Or: logical operator, and is used to combine conditional statement **
 ** Logical Operator in Java: && and ||.

If statements cannot be empty, but you can use pass keyword statements to avoid getting an error.

Loops
    Primitive loop: While loops and For Loops.

While Loop:
    With the while loop we can execute a set of statements as long as a condition is true.
    While loop requires relevant variables to be ready which is define variable i = 1, then increment it later as long as a condition we defined above is true.
For Loop:
    For loop is used for iterating over a sequence (list, tuple, dictionary, set or string).


#####################################################################
#####################################################################
Data Structure:

---------------------------------------------------------------List:
Lists are used to store multiple items in a single variable
myList = [1, 2, 3]
print(myList) → [1, 2, 3]
List items are ordered, changeable, and allow duplicate values. 

The list() Constructor → it is also possible to use the list() constructor when creating a new list. 

Access items in list: since lists are indexed and you can access them by referring to the index number.
myList = [“Long”, “Nguyen”, “Huu”, “Huy”]
print(myList[2]) → [“Huu”]

Negative Indexing: Negative Indexing means start from the end. -1 refers to the last item
myList = [“Long”, “Nguyen”, “Huu”, “Huy”]
print(myList[-3]) → [“Nguyen”]

Check if Item Exists: we use in keyword to determine if a  specified item is present in a list.

Insert Items: to insert a new list item, we can use insert() method.
insert() method takes 2 parameters, index and value. 

Append Items: to add an item to the end, we can use append() method.

Extend List: we can use extend() method to append elements from another list to the current list.

myCurrList = [“Long”, “Nguyen”]
myExtendList = [“Huu”, “Huy”]
myCurrList.extend(myExtendList)
print(myCurrList) → [“Long”, “Nguyen”, “Huu”, “Huy”]

→ you can use extend() method to append different iterable collections such as tuples, sets, or dictionaries.

Remove Specified Item: remove() method is used to remove a specified item.
Remove Specified Index: pop() method is used to remove the specified index.

Clear the List: clear() method is used to clear the content of the list, but the list still remains.

Loop Through a List: we can use for loop with this syntax:
myList = [ ‘Long’, ‘Nguyen’, ‘Huu’, ‘Huy’ ]
for x in myList:
	print(x) → Long Nguyen Huu Huy

Loop Through the Index Numbers: most use to loop through the list items by referring to their index number. We use range() and len() methods to create a suitable iterable.
myList = [ ‘Long’, ‘Nguyen’, ‘Huu’, ‘Huy’ ]
for i in range(len(myList))
	print(myList[i])

Using a While Loop: 
Beside for loop, we can use while loop to loop through the list items. 
Use the len() function to determine the length of the list, then start at 0 and loop your way through the list items by referring to their indexes. 
Remember to increase the index by 1 after each iteration.
myList = [ ‘Long’, ‘Nguyen’, ‘Huu’, ‘Huy’ ] 
i = 0
while i < len(myList)
	print(myList[i])
	i += 1
Comprehension Loop: 
myList = [ ‘Long’, ‘Nguyen’, ‘Huu’, ‘Huy’ ]
[ print(x) for x in myList ]
Comprehension loop offers shorter syntax.

Sort Lists:
We can use sort() method, it will sort the list alphanumerically, ascending, by default
If we want to sort descending order, we can use sort(reverse = True)
We can customize sort function by using the keyword argument key = function
→ sort( key = myFunc)

Copy a List:
You cannot copy a list simply by: list2 = list1, because list2 is just pointing at the reference of list1. Once list1 is changed, list2 is also changed. 
We can use copy() method, or list() method.


-------------------------------------------------------Tuple:
Tuples are used to store multiple items in a single variable. 
A tuple is a collection which is ordered and unchangeable.

Change Tuple Values:
Since tuple is ordered and unchangeable, we can do this:
Convert a tuple to a list, then change the value of this list, then convert the list back to tuple.
Tuple → list → modify value: list → tuple.
Similar to modify, add and remove we can convert tuples to lists and convert back to tuples.
Tuple Methods: count() and index()
count() returns the number of times a specified value occurs in a tuple.
index() searches the tuple for a specified value and returns the position of where it was found.

------------------------------------------------------Set:
Set is a collection which is unordered, unchangeable, and unindexed.
Unordered - do not have a defined order. Set will appear different every time you use them and cannot be referred to by index or key.
Unchangeable - once created, you cannot modify the items, but you can add or remove items.

Access Items
We can loop through the set using for loop.

Add Items
To add items in a set, we can use the add() method.

Add Another Set to Current Set
update() method is used to add another set to the current set.

Remove Item
We can use either remove() or discard() method.
Another way to remove an item using pop(), but it will randomly remove any item. → Because the set is unordered, so you don’t know which item gets removed.

Join 2 Sets
We can use Union() method to return a new set. Syntax:
Set1 = { 1, 2, 3 }
Set2 = {‘a’, ‘b’, ‘c’}
Set3 = set1.union(set2) → {1, 2, 3, ‘a’, ‘b’, ‘c’}

Or we can use update().
→ These two methods will keep only unique values.

Keep Only the Duplicates:
We can use intersection_update(). Syntax:
X = {1, 2, 3}
Y = {2, 4, 6}
x.intersection_update(y) → { 2 }

Or we can use intersection() that keeps only unique values contained in both sets and return a new set.

Keep All, but NOT the Duplicates:
The symmetric_difference_update() is used to keep only the elements that are NOT present in both sets.

The symmetric_difference() method is also used to keep elements that are NOT present in both sets and return a new set.

----------------------------------------------------Dictionary:
Dict is used to store data values in key:value pairs. 
→ ordered, changeable, do not allow duplicates. 
Similar to HashMap in Java – syntax:
myDict = { 
	“Brand”: “Chev”
	“Model”: “LS”
	“Year”: 1964
}

Accessing Items:
We can directly use square brackets myDict[“Year”] to access dictionary
Or we can use get() method.

Get Keys:
The keys() method will return a list of all the keys in the dictionary.

Get Items:
The items() method will return each item in a dictionary, as tuples in a list.

Change Value:
Directly change value with this syntax: myDict[“Year”] = 1997

Update Dictionary:
We can use update() method to update the dictionary.
update() take an argument and it must have a key:value pairs.


Add Items:
Something similar to change value, but instead we add a new attribute to the dictionary.

Removing Items:
We can use pop() method to remove the item with the specified key name.
popitem() method is also used to remove the last inserted item. 
Or we can just use keyword del.

Loop:
We can use for loop to loop through a dict, depends on the purpose of your loop:
myDict.keys() → return all keys of your dictionary.
myDict.values() → return all values of your dictionary.
myDict.items() → return all key:value pairs. **syntax: for x, y in myDict.items() → print(x,y)

Copy:
Dict, Set, List: similar to Object in Java. Dict1 = Dict2 only pointing to Dict2’s reference.
So we have to use copy() method or dict() method.

Nested Dictionaries:
A dictionary can contain a dictionary, this is called nested dictionaries.
Access: straightforward with this syntax: print(myDict[“child2”][“name”])


#####################################################################
#####################################################################
Module:
Basically any file extension with this .py can be a module. 
Module is similar to code library – a file contain set of functions you want to include in your application. 

Variables in Module:
Module can have functions, also variables of all types (arrays, dicts, sets, lists, objects)
To access these variables, you must define a new variable and call the module name along with the variable.
→  a = mymodule.person1[“age”]

Rename: 
Using keyword as to rename the module.


#####################################################################
#####################################################################

Exceptional Handling
The try block lets you test a block of code for errors
The except block lets you handle the error. ** Java uses catch, Python uses except
The else block lets you execute code when there is no error.
The finally block lets you execute code, regardless of the result of the try- and except blocks.
