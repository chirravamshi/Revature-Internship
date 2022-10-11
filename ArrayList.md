## ArrayList
- It is a part of collection framework that provides dynamic arrays in java.
- It is an index based collection

### Array VS ArrayList
- ArrayList is slower than standard array. when a array is created the length of array can't be changed.
- ArrayList has variable length.
- ArrayList can only store objects. Primitives are automatically converted into object via auto boxing.

### Declaration of ArrayList

**Syntax:** ArrayList<classname> arrayList = new ArrayList<>(); //
**Example:**
```java
ArrayList<Integer> arrayList = new ArrayList<>();
```
### ArrayList Methods
- size() - It returns a integer that shows the size of the arraylist
- get() - It is used to get element from specified index within the list.
- set() - It is used to set the value at the given index of the list and the previous value is replaced by the new value.
- add() - It adds elements to the arraylist.
- contains() - It returns boolean that shows the element present or not.
- isEmpty() - It returns boolean that shows the arraylist has any elements or not.
- indexOf() - It returns the index of first occurrence.
- lastIndexOf() - It returns the index of last occurrence.

### Example
```java
    ArrayList<Integer> arrayList = new ArrayList<>();
	arrayList.add(2);
	arrayList.add(10);
	arrayList.add(4);
	int a = 10;
	arrayList.add(a);                               //using variable
	arrayList.add(a-4);
	System.out.println(arrayList);                      //[2, 10, 4, 10, 6]
	System.out.println(arrayList.size());               //5
	System.out.println(arrayList.get(2));               //4
	arrayList.set(2, 34);                               //-> replaces 4 by 34
	System.out.println(arrayList);                      //[2, 10, 34, 10, 6]
	System.out.println(arrayList.contains(34));         //true
	System.out.println(arrayList.isEmpty());            //false
	System.out.println(arrayList.indexOf(10));          //1
	System.out.println(arrayList.lastIndexOf(a));       //3
    //regular for loop to access the elements of arraylist
    for (int i = 0; i < arrayList.size(); i++) {
			System.out.print(arrayList.get(i) + " ");   //2 10 34 10 6
	}
    //advaced for loop to access the elements of arraylist
	for(int i:arrayList) {
			System.out.print(i + " ");                  //2 10 34 10 6
	}
```