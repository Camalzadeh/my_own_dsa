# My Own DSA

One generic `MyList<T>` interface, implemented twice - once over a resizing array
and once over linked nodes - so the same test routine can drive both.
Java Lessons, task 4.

## What it covers

- A generic interface with `add`, `insert`, `set`, `get`, `remove` (by index and by
  value), `contains`, `size`, `isEmpty` and `clear`.
- `MyArrayList` - backed by an array that grows when it fills.
- `MyLinkedList` - backed by singly linked nodes.
- `Iterable<T>`, so both work in a `for (String s : list)` loop.
- `bubbleSort()` and a `toString()` that prints the contents.

`Main.implement()` runs an identical sequence of operations against each
implementation; the two outputs should match line for line. That is the test.

## Running it

```bash
javac -d out src/*.java
java -cp out Main
```

## Layout

- `src/MyList.java` - the interface.
- `src/MyArrayList.java`, `src/MyLinkedList.java` - the two implementations.
- `src/Main.java` - the shared exercise routine.
