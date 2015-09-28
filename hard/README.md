# Binary Bonanza


Write the function printb() (in C!) that takes a pointer to a 4 byte value and prints its binary representation (preceded by `0b`).

```c
int main (int argc, char **argv) {

  int    a = 42;
  float  b = 13.37;

  printb(&a);
  printb(&b);

  return 0;
}

void printb (void *p) {
  // ... your code here ...
}
```

Brownie-points: Don't print out any of the leading zeros!

--------------------------------------------------------------------

# The Seg Fault in our Char Stars

Lenny wanted to check his understanding of strings in C and pointers, and he wrote the following code

```c
#include <stdio.h>

int main(int argc, char **argv)
{
	char **s;
	char foo[] = "Hello World";

	*s = foo;
	printf("s is %s\n", (char *)s);

	s[0] = foo;
	printf("s[0] is %s\n", s[0]);
	return 0;
}
```
What happens with this program is run? Can you figure out on what line the error(s) occurs, and why?