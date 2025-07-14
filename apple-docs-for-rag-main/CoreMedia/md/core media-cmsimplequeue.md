

- Core Media
-  CMSimpleQueue 

Class

# CMSimpleQueue

A reference to an instance that provides a simple lockless queue of elements.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
class CMSimpleQueue
```

## Topics

### Managing Queues

func enqueue(UnsafeRawPointer) throws

Enqueues an element in the queue.

func dequeue() -> UnsafeRawPointer?

Dequeues an element from the queue.

func reset() throws

Resets the queue.

### Inspecting Queues

var head: UnsafeRawPointer?

The head element in the queue.

var capacity: Int

The number of elements that a queue can hold.

var count: Int

The number of elements currently in the queue.

var fullness: Float

The fullness of a queue as a percentage of its capacity.

### Accessing the Type Identifier

static var typeID: CFTypeID

The type identifier of sample buffer objects.

### Errors

struct Error

A structure that defines errors that queue operations can produce.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

