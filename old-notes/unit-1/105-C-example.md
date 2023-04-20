# C code example

1. Open a terminal window.<br>

2. Create a new folder with mkdir:<br>
~~~~html
  $ mkdir exercise_C
  $ cd mkdir exercise_C
~~~~


2. Let us edit a new file:<br>
~~~~html
  $ vim hola.c
~~~~

3. Press the 'i' key to edit the file, and add the following lines.<br>

4. Now, let us check which environment you have:<br>
~~~~html
#include <stdio.h>
int main() {
printf("Hola Mundo.\n");
return 0;
}
~~~~

5. This program will will print a string of characters on the screen, but we need to compile it first.<br>
~~~~html
  $ gcc -o hola.exe hola.c
~~~~

6. This creates an executable file called hola.exe. To run the program we created:<br>
~~~~html
  $ ./hola.exe
  Hola Mundo.
~~~~

And this is our first C program.