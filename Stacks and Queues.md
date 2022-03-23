﻿﻿﻿# Week 4 - Stacks and Queues

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

### Activity 1: LIFO vs FIFO

Record your answer here

### Activity 2: Stacks and LIFO

Record your answer here

### Activity 3: Pushes and pops

Record your answer here

### Activity 4: Communication through a linked list

Record your answer here

### Activity 5: FIFO and queues

Record your answer here

### Activity 6: Arrays, linked lists, and queues

| Operation | Array |   Linked List  |
| --------------------------------- | --------------- | -------------- |
| Insert / remove **first **element |                 |	|
| Insert / remove **last**element   |                 | 	|
| Peek first / last element         |                 |	|

Record your answer here

### Activity 7: Time complexities, once again

| Operation                     | Time complexity |
| ----------------------------- | --------------- |
| Insert / remove first element |                 |
| Insert / remove last element  |                 |
| Peek first / last element     |                 |


Record your answer here

### Activity 8: Buffer initialization

```c
// version 1
void buffer_init(buffer_t *queue, size_t capacity) {
    queue->head = queue->count = 0;
    queue->data = (char*) malloc(capacity * sizeof(char));
    if (queue->data != NULL) queue->capacity = capacity;
    else queue->capacity = 0;
}

// version 2
void buffer_init(buffer_t *queue, size_t capacity) {
    char data[capacity;]
    queue->head = queue->count = 0;
    queue->data = data;
    queue->capacity = capacity;
}
```

Program to test:

```c
int main(void) {
	buffer_t queue;
	buffer_init(&queue, 100);
	for (int i = 0; i < 100; i++) queue->data[i] = '?';
	buffer_destroy(&queue);
}
```

Record your answer here

### Activity 9: Clock arithmetic

```c
size_t buffer_rear(const buffer_t * queue) {
}
```

Record your answer here

### Activity 10: Writing into a circular buffer

```c
void buffer_write(buffer_t * queue, char value) {
}
```

Record your answer here

### Activity 11: Reading from a circular buffer

```c
char buffer_read(buffer_t * queue) {
}
```

Record your answer here

### Activity 12: Testing the queue

```c
int main(void) {
    buffer_t buffer;
    buffer_init(&buffer, 10);
    char c = getchar();
    while (c != '#') {
	    if (c == '*') printf("Read: '%c'\n", buffer_read(&buffer));
	    else if (c != '\n') buffer_write(&buffer, c);
	    c = getchar();
    }
    buffer_destroy(&buffer);
    return 0;
}
```



Record your answer here

### Activity 13: Fullness and emptiness

```c
// returns 1 if the buffer is full, 0 otherwise
int buffer_full(const buffer_t * queue) {
}

// returns 1 if the buffer is empty, 0 otherwise
int buffer_empty(const buffer_t * queue) {
}
```

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
