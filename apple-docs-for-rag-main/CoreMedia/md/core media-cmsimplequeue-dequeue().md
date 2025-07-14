

- Core Media
- CMSimpleQueue
-  dequeue() 

Instance Method

# dequeue()

Dequeues an element from the queue.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func dequeue() -> UnsafeRawPointer?
```

## Return Value

A pointer to a dequeued element.

## See Also

### Managing Queues

func enqueue(UnsafeRawPointer) throws

Enqueues an element in the queue.

func reset() throws

Resets the queue.

