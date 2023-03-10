# Arduino Library Template
```MyLibrary.h```
 
```cpp
#ifndef MyLibrary_h
#define MyLibrary_h

#include "Arduino.h"
class MyLibrary 
{
	public:
	MyLibrary();
	void begin();
	void doSomething();
private:
	int _variable;
};
#endif
```
The ```#ifndef``` and  ```#define``` directives are used to prevent the library from being included multiple times.

### Here is the implementation code for the library

```MyLibrary.cpp```

```cpp
#include "MyLibrary.h"
MyLibrary::MyLibrary() {
// Constructor code
}
void MyLibrary::begin() {
// Initialization code
}
void MyLibrary::doSomething() {
// Function code
}
```
In this code, the constructor initializes any necessary variables, the begin() function performs any necessary initialization, and the doSomething() function performs some specific action.

#### Once you have written the library, you can include it in your Arduino sketch by adding the following line at the top of your sketch
```cpp 
#include <MyLibrary.h>
 ```
 Then, you can create an instance of the MyLibrary class and call its functions
 ```cpp
 MyLibrary myLibrary;

void setup() {
	 myLibrary.begin();
}

void loop() {
	 myLibrary.doSomething();
}
```