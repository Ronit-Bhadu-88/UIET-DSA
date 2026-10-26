# Heap Sort

This folder contains two C++ examples of heap sort:

- `Heap_Sort.cpp` sorts an array of integers.
- `Heap_Sort_Linked_List.cpp` sorts the values stored in a singly linked list.

## How heap sort works

Heap sort uses a **max heap**, where each parent is greater than or equal to
its children:

1. Build a max heap from the values.
2. Swap the largest value at the root with the last value in the heap.
3. Reduce the heap size and restore the max-heap property.
4. Repeat until the values are sorted in ascending order.

The running time is **O(n log n)**.

## Linked-list example

A linked list does not support the fast indexed access needed to use the usual
array-based heap directly. This example copies the list's values into a vector,
heap-sorts the vector, and copies the sorted values back into the list nodes.
The list's nodes stay in their original positions.