

- Core Media
- CMSimpleQueue
-  enqueue(\_:) 

Instance Method

# enqueue(\_:)

Enqueues an element in the queue.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func enqueue(_ element: UnsafeRawPointer) throws
```

## Parameters 

`element`  

The element to enqueue.

## See Also

### Managing Queues

func dequeue() -> UnsafeRawPointer?

Dequeues an element from the queue.

func reset() throws

Resets the queue.

