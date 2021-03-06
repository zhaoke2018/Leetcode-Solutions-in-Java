# Java Data Structure Cheatsheat

## Array
[Ref](https://www.geeksforgeeks.org/array-vs-arraylist-in-java/)
### New
```Java
//Declaration Syntax
int[] Array1; //First choice
int Array2[]; 

//Initialization Syntax
int[] myArray1 = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
int[] myArray2 = new int[] {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
int[] myArray3 = new int[10];
```
### For-Each Loop
```Java
for(type element: array) {
    System.out.println(element);
}
```
### Multi dimensional arrays
```Java
//two-dimention array
type[][] typeName = new type[typeLength1][typeLength2];
```
### Big-O Efficiency
* Indexing: O(1)
* Search: O(n)
* Optimized Search: O(log n)
* Insertion: n/a

### Array vs. ArrayList
1. Array size is fixed, but ArrayList size is dynamic.
```java
int[] arr = new int[10];
ArrayList<Type> arrL = new ArrayList<Type>();
```
2. Array members are accessed using [], while ArrayList has a set of methods to access elements and modify them.
3. Array can contain both primitive data types as well as objects of a class depending on the definition of the array. However, ArrayList only supports object entries, not the primitive data types. Since ArrayList can’t be created for primitive data types, members of ArrayList are always references to objects at different memory locations.References of the actual objects are stored at contiguous locations. In array, it depends whether the arrays is of primitive type or object type. In case of primitive types, actual values are contiguous locations, but in case of objects, allocation is similar to ArrayList.

### Arrays Methods
```Java
Arrays.sort(a);//ascending, O(n log(n))
Arrays.equals(a, a2);
Arrays.toString();
```
## Queue
[Ref](https://leetcode.com/explore/learn/card/queue-stack/228/first-in-first-out-data-structure/1367/)
```java
public class Main {
    public static void main(String[] args) {
        // 1. Initialize a queue.
        Queue<Integer> q = new LinkedList();
        // 2. Get the first element - return null if queue is empty.
        System.out.println("The first element is: " + q.peek());
        // 3. Push new element.
        q.offer(5);
        q.offer(13);
        q.offer(8);
        q.offer(6);
        // 4. Pop an element.
        q.poll();
        // 5. Get the first element.
        System.out.println("The first element is: " + q.peek());
        // 7. Get the size of the queue.
        System.out.println("The size is: " + q.size());
    }
}
```
