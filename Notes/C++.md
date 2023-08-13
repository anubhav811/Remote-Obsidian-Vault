
***IO***
```
<<  Insertion operator
>> Extraction operator
```

***Header Files***
**System defined header files -> comes with compiler**

 ```
 #include <iostream>
```

**User defined header files -> by programmer**
 ```
 #include "this.h"
```

***Scope resolution operator***

```
int c = 5;
int main(){
	int c = 2;
	cout<<c;  // will output 2
	cout<<::c // will output 5
}
```

***Float, double and long double literals***
```
size of double   -> 8
size of float -> 4
size of long double/float -> 12
```

***Reference Variables***
```
int x = 5;
int &y = x;
cout<<x<<endl;
cout<<y<<endl;
```

**Output**
```
5
5
```

***Pointers***
```
int a = 3;
int* b = &a;

& -> "address of"
* -> dereference

// Pointer to pointer
int** c = &b;

cout<< &a -> address of a
cout<< b  -> address of a
cout<< *b -> value at address of a or simple value of a
cout<< &b -> address of b (which stores address of a)
cout<< c  -> address of b (which stores address of a)
cout<< *c -> value of b (which is the address of a)
cout<< **c -> value stored at , value stored at b (value of a) 
```

**Pointer Arithmetic**
```
int marks[4] = {32,99,38,51};
int* p = marks ;
cout<< p ;     \\ address of first element marks[0]
cout<< *p ;    \\ value of first element ->32
cout<< *(p+1) ; \\ 99
cout<< *(p+2) ; \\ 38
cout<< *(p+3) ; \\ 51
```

**typdef***
```
typedef <type> <name> ; 

example

typedef struct emp{
	int eId;
	char favChar;
	float salary;
} ep;

type -> struct emp....
ep -> name
```
