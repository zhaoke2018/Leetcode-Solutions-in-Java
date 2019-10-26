# Java Data Structure Cheatsheat

## Array

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

### Array, ArrayList

### Arrays
Arrays.sort(a);//ascending, O(n log(n))
Arrays.equals(a, a2);
Arrays.toString();
