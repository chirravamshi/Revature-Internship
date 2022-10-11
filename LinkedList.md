## LinkedList
- Linkedlist is index based collection framework.
## Arraylist vs LinkedList
- ArrayList is fast for storing the elements and accessing the elements from the list.
- LinkedList is fast for inserting and deleting the elements from the list.

### Declaration of LinkedList

**Syntax:** LinkedList<classname> listList = new LinkedList<>(); //
**Example:**
```java
LinkedList<Integer> linkedList = new linkedList<>();
```
### List Methods
- size() - It returns a integer that shows the size of the arraylist
- get() - It is used to get element from specified index within the list.
- set() - It is used to set the value at the given index of the list and the previous value is replaced by the new value.
- add() - It adds elements to the arraylist.
- contains() - It returns boolean that shows the element present or not.
- isEmpty() - It returns boolean that shows the arraylist has any elements or not.
- indexOf() - It returns the index of first occurrence.
- lastIndexOf() - It returns the index of last occurrence.
- remove() - It removes the element at the given index.
- removeFirst() - It removes the element in first index.
- removeLast() - It removes the element in last index
- getFirst() - It gives first index value.
- getLast() - It gives last index value.

### Example
```java
	LinkedList<Integer> linkedList = new LinkedList<>();
	linkedList.add(2);
	linkedList.add(10);
	linkedList.add(4);
	int a = 10;
	linkedList.add(a);
	linkedList.add(a-4);
	System.out.println(linkedList);                 //[2, 10, 4, 10, 6]
	System.out.println(linkedList.size());          //5
	System.out.println(linkedList.get(2));          //4
	linkedList.set(2, 34);                          //->replaces 4 by 34
	System.out.println(linkedList);                 //[2, 10, 34, 10, 6]
	System.out.println(linkedList.contains(34));    //true
	System.out.println(linkedList.isEmpty());       //false
	System.out.println(linkedList.indexOf(10));     //1
	System.out.println(linkedList.lastIndexOf(a));  //3
	System.out.println(linkedList.remove(1));       //10
	System.out.println(linkedList.removeFirst());   //2
	System.out.println(linkedList.removeLast());    //6
	System.out.println(linkedList.getFirst());      //34
	System.out.println(linkedList.getLast());       //10
    //regular for loop to access the elements of linked list
    for (int i = 0; i < linkedList.size(); i++) {
		System.out.print(linkedList.get(i) + " ");  //34 10
	}
    //advaced for loop to access the elements of linked list
	for(int i:linkedList) {
		System.out.print(i + " ");                  //34 10
	}
    ```