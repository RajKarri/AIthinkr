# Arrays in high level languages like C#

[Home](index.md)&emsp;[About Me](about-me.md)

1) An array is a collection of similar elements.
2) Array runs from 0 to n-1 where n is the length of array.
3) Arrays are reference types, not value types. <kbd>null</kbd> can be assigned to an array.   
   ```
   int[] test_array = null;
   ```
4) Array elements can be value types or reference types, but array is always a reference type. As arrays are reference types, array holds the reference but not the actual value. 
   ```
   int[] test_array_1 = new int[5]; // Array with value type of elements
   Student[] test_array_2 = new Student[5] // Array with reference type of elements
   ```  
5) Length is required during Array initialization, and it is fixed. One can neither allocate or de-allocate memory after initialized.
   ```
   int[] test_array_1 = new int[5]; //  Length is 5. Array runs from 0 to 4 (5 elements)
   ```   
**Example:**

Imagine a customer booking 5 non-cancellable tickets in a plane for his family.
```
  // Length 5 must be provided during initialization. One can't initialize array without providing length.
  Ticket[] my_family_tickets = new Ticket[5]; 
```
Here 5 tickets are allotted to family. Irrespective of number of family members went on trip, all tickets will consider as utilized.

So, ideally one shouldn't use arrays when not sure about the length during initialization or usage of all elements.

