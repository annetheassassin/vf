﻿﻿# Week 3 - Linked Lists

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

### Activity 1: Pointers to pointers

Record your answer here

| Variable    | Address               | Value |
| ----------- | --------------------- | ----------- |
| value       |                       |  |
| ptr         |                       |  |
| pptr        |                       |  |
| ppptr       |                       |  |

### Activity 2: Chaining pointers

```c
typedef struct node_t {
	int value;
	struct node_t * next;
} node;

int main(void) {
	node fourth = {.value = 42, .next = NULL};
	node third = {.value = 7, .next = &fourth};
	node second = {.value = 3, .next = &third};
	node first = {.value = 2, .next = &second};
	
	printf("first: %d\n", first.value);
	printf("second: %d\n", (*(first.next)).value);
	printf("third: %d\n", (*(*first.next).next).value);
	printf("fourth: %d\n", (*(*(*first.next).next).next).value);
}
```
Record your answer here

### Activity 3: Traversal

```c
int main(void) {
	node fourth = {.value = 42, .next = NULL};
	node third = {.value = 7, .next = &fourth};
	node second = {.value = 3, .next = &third};
	node first = {.value = 2, .next = &second};
	
	for (/*init*/; /*condition*/; /*advance*/) {
		printf("%d\n", /*current value*/);
	}
}
```

Record your answer here

### Activity 4: Linked list deallocation

Record your answer here

```c
void list_free(list ** plist) {
	free(*plist);
	*plist = NULL;
}
```

### Activity 5: Prepending

Record your answer here

```c
void list_prepend(list * plist, int value);
```

### Activity 6: Time complexity of prepend and append

Record your answer here

### Activity 7: Access by index

Record your answer here

```c
// returns the node at index 'index' in the list referred to by pList
const node *list_at(const list *plist, int index);
```

### Activity 8: Time complexity of accessing by index

Record your answer here

### Activity 9: A bad for-loop

Record your answer here

### Activity 10: Removal in a singly-linked list

Record your answer here

```c
void list_remove_last(list * plist) {
	node_free(&list->tail);
}
```

### Activity 11: Code update - I


Record your answer here

### Activity 12: Code update - II

Record your answer here

### Activity 13: Implementation of removal

Record your answer here

```c
// updates the list by removing the node referred to by pnode from the list
void list_remove(list *plist, node *pnode) {
	pnode->prev->next = pnode->next;
	pnode->next->prev = pnode->prev;
	pnode->next = pnode->prev = NULL;
}
```

### Activity 14: Implementing insertion

Record your answer here

```c
// updates the list by inserting value before the node referred to by pInsertionPoint
void list_insert(list *plist, node *pbefore, node *pnode) {
    
}
```

### Activity 15: Time complexities

Record your answer here

| Operation       | Array                      | Linked List |
| --------------- | -------------------------- | ----------- |
| Access          |                            | |
| Append          |                            | |
| Insert          |                            | |
| Remove          |                            | |


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
