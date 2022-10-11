## Strings
    It is an object that represents the sequence of characters.

## Declaring Strings
```java
    String name = "John"; ///
    String name = new String("John");
	//converting characters array into string
    char[] ch = {'J','o','h','n'};
	String string = new String(ch);
```
## With & Without new
When "new" is used the value store in the heap memory.
    Without "new" the value stored in the String pool.
    The usage of the operator "==" for two strings with same values will return false where "==" compares value and reference;

### Example
```java
    char[] ch = {'w','o','r','d'};
	String string = new String(ch);
	System.out.println(string);                 //word
	String string2 = "word";
	String string3 = new String("word");    
	String string4 = "word";
	System.out.println(string==string2);        //false
	System.out.println(string3==string2);       //false
	System.out.println(string3==string);        //false
	System.out.println(string2==string4);       //true
    System.out.println(string3.equals(string)); //true
	```
	
## String Methods
- length - It returns the length of the string.
- stringCompare() - It returns an integer based on the two given. It returns 0 when the value two strings are the same.
- equals() - It returns true or false based on the two string value
- cancat() - It returns a string combination of two string into one.
- split() - It is mostly used to slip the single to string array.
- replace() - It replace the all occurance of the string which is given.
- substring() - It returns the string from another string

### Example
```java
     String string = "Eaxmple";
	 String string2 = "Eaxmple2.0";
	 String string3 = "Eaxmple";
	 String string4 = "Eaxmple for split function";
	 System.out.println(string.length());               //7
	 System.out.println(string.compareTo(string2));     //-3
	 System.out.println(string.equals(string3));        //true
	 System.out.println(string.concat(string2));        //EaxmpleEaxmple2.0        
	 String[] arrstr = string4.split(" ");                  
	 System.out.println(Arrays.toString(arrstr));       //[Eaxmple, for, split, function]
	 System.out.println(string4.replace(" f","_3"));    //Eaxmple_3or split_3unction
	 System.out.println(string4.substring(4,12));       //ple for 
```