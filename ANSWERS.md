
# Answer Document

##### Andrew ID: andrew_id

## Part 1: Practice Problems (15%)
### Question 1


Given a pointer to struct D called “d”, what expression will access “data”, the member of struct A? You may assume that all pointers are initialized and are valid.

```cpp
struct A {
    float data;
};

struct B {
    A a;    
};

struct C {
    B* b;
};

struct D {
    C c;
};
```

#### Answer
Insert answer here

### Question 2


Given the following structs, predict the memory layout of a struct A named “stack”. You may assume that it is a 32-bit machine.


```cpp
struct A{
    float a, b, c;
    B* ptr;
    B mem;
};

struct B {
    float d, e;
};

A stack;
```


| Address | Expressions
| --- | --- |
| A+0x0 | stack, stack.a |
| A+0x | |
| A+0x | | 
| A+0xC | |
| A+0x | |
| A+0x | |


#### Answer


| Address | Expressions
| --- | --- |
| A+0x0 | stack, stack.a |
| A+0x | |
| A+0x | | 
| A+0xC | |
| A+0x | |
| A+0x | |


### Question 3

Given the functions below, what is the value stored  in the points a and b after calling foo?

```cpp
struct point {
    float x, y;
};

void foo(point& p1, point p2) {
    point p3;
    p3.x = p1.x + p2.x;
    p3.y = p1.y + p2.y;
    bar(p3);
    p1.x -= p3.x;
    p1.y -= p3.y;
}

void bar(point p3) {
    p3.x *= .5f;
    p3.y *= .5f;
}

point a, b;
a.x = b.y = 1;
a.y = b.x = 0;
foo(a, b);
```

#### Answer

Insert answer here

## Part 2: Coding Questions

### Question 1 


Write an overview of how your AI works, including how it detects where projectiles will fall and how it chooses where to go.

#### Answer

Insert answer here

### Question 2



What challenges did you face when writing an AI?
#### Answer

Insert answer here

### Question 3

How well does your AI work on a Hard scenario? If it doesn’t work, why? If it does, try harder scenarios and see when it does fail and explain why?


#### Answer
Insert answer here

### Question 4

What did you think of the assignment and did it meet its goals? Why or why not?


#### Answer