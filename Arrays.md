## Arrays 

- Array is a group similar type variables that represented by a common name.
- The elements are stored at memory in squencial manner.
- The size of the array is fixed.
- By using the index, the values of the array can be accessed.
- Default value of undefined array at any index is 0. 

### Declaring a variable

**Syntax:** datatype[] arrayname = new arrayname[size];

### Example
```java
    int[] a = new int[10];
    char[] ch = new char[n];    //n is a variable

    //Creating Scanner Object to get input the user
    //make to import java.util package whenever you use scanner
    Scanner input = new Scanner(System.in);

    // To get the array elements form the user
    for(int i=0;i<n;i++){  
        a[i]=input.nextInt();    
    }
            
    char[] ch = {"j", "o", "h", "n"};   // while declaring
```

- Array length - It returns the length of the array

**Example**
   ```java
        int[] a= {4,7,3,1,3,2}; 
        System.out.println(a.length); //output =>  6
```
**Accessing the elements**
```java
        int[] a= {4,7,3,1,3,2};
	    System.out.println(a[1]+a[2]);//10  =>by using index
	    System.out.println(a[0]+a[2]);//7   
```

## Arrays class
- It is part of Java collection framework in java.util package. 
- It provides static methods that are used for java arrays.

### Methods of Arrays class
```java
    int[] a= {4,7,3,1,3,2}; 
	  Arrays.sort(a);  //the array elements are replaced  the sorted elements
	  System.out.println(Arrays.toString(a));
	  System.out.println(Arrays.binarySearch(a, 3));
	  System.out.println(Arrays.binarySearch(a, 3, 5, 3));
``` 
    Output
        [1, 2, 3, 3, 4, 7]   //the string show array values 
        2                    //to find the first found of the element.
        3                    //to find the element from start to end in the form of (array,start,end,key)

## 2D Array
- 2D Array is used to defined values in the form of rows and columns or matrix form.

### Example
```java
    int[][] a = new int[4][5];

    Program for transfers
    int[][] a = {{1,2,3},{4,5,6},{7,8,9},{10,11,12}};
	  for(int i=0;i<3;i++) {
		  for(int j=0;j<4;j++) {
			  System.out.print(a[j][i]+" ");
		  }
		  System.out.println();
	  }
    }
```
    Output
    1 4 7 10 
    2 5 8 11 
    3 6 9 12 

    

