﻿# Week 2 - Dynamic Arrays

## Team

Team name:
Date:

Members

| Role                                                                                                                                                                          | Name |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| **Facilitator** keeps track of time, assigns tasks and makes sure all the group members are heard and that decisions are agreed upon.                                             |      |
| **Spokesperson** communicates group’s questions and problems to the teacher and talks to other teams; presents the group’s findings.                                              |      |
| **Reflector** observes and assesses the interactions and performance among team members. Provides positive feedback and intervenes with suggestions to improve groups’ processes. |      |
| **Recorder** guides consensus building in the group by recording answers to questions. Collects important information and data.                                                   |      |

## Activities
Make sure to have the activities signed off regularly to ensure progress is tracked.

Set up a project in CLion to write the small programs needed in some of the activities.

### Activity 1: Random access

````c
#include <stdio.h>
#define COUNT (50)

void fill_fibonacci(unsigned long long * storage, int count) {
	*storage = 0;
	*(storage + 1) = 1;
	for (int i = 2; i < count; i++) {
		*(storage + i) = *(storage + i - 1) + *(storage + i - 2);
	}
}

int main(void) {
	unsigned long long array[COUNT];
	fill_fibonacci(array, COUNT);
	for (int i = 1; i < COUNT; i++) {
		printf("f(%d) = %llu\n", i, array[i]);
	}
}
````



### Activity 2: Array definition
This is how you include code listings in your markdown document:
```C
typedef struct array {
    size_t capacity;
    size_t count;
    float *data;
} array_t;
```
Record your answer here

### Activity 3: Correct initialization

```C
array_t *array_init(array_t *pArray, size_t capacity);
```
Record your answer here


### Activity 4: Cleaning up

```c
int main(void) {
    
}
```



Record your answer here

### Activity 5: Resizing an array

```c
void array_reserve(array *p_array, size_t min_capacity) {
    size_t capacity = p_array->capacity;
    while (capacity < min_capacity) {
        capacity = (capacity + 1) * ...
    }
    /* reallocate memory, update capacity of array, etc. */
}
```



Record your answer here

### Activity 6: Appending values

```c
void array_append(array * arr, float value);
```

Record your answer here

### Activity 7: Inserting values

```c
void array_insert(array * arr, int index, float value);
```

Record your answer here

### Activity 8: Removing by index

```c
void array_remove(array * arr, int index);
```

Record your answer here

### Activity 9: Finding a value

```c
int array_find(const array * arr, float value);
```

Record your answer here

### Activity 10: Constant time complexity

Record your answer here

### Activity 11: Worst-case time complexity

| Operation       | Worst-case time complexity |
| --------------- | -------------------------- |
| Insert          |                            |
| Remove          |                            |
| Find            |                            |
| Lookup / access |                            |

Record your answer here

### Activity 12: Complexity of *append*

Record your answer here

### Activity 13: Storing grades in a dynamically growing array

Record your answer here


## Looking back

### What we've learnt

Formulate at least one lesson learned.

### What were the surprises

Fill in...

### What problems we've encountered

Fill in...

### What was or still is unclear

Fill in...

### How did the group perform?

How was the collaboration? What were the reasons for hick-ups? What worked well? What can be improved next time?





> Written with [StackEdit](https://stackedit.io/).
