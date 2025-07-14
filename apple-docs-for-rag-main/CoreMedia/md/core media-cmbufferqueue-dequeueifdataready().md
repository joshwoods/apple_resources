

- Core Media
- CMBufferQueue
-  dequeueIfDataReady() 

Instance Method

# dequeueIfDataReady()

Dequeues a buffer from the queue, if it’s ready.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func dequeueIfDataReady() -> CMBuffer?
```

## Return Value

A buffer or `nil` if the buffer is empty or the data isn’t ready.

## See Also

### Managing a Queue

func enqueue(CMBuffer) throws

Enqueues a buffer to the queue.

func dequeue() -> CMBuffer?

Dequeues a buffer from the queue.

func markEndOfData() throws

Marks a buffer as being at the end of its data.

func reset() throws

Empties the queue and resets its end-of-data state.

func reset((CMBuffer) throws -> ()) throws

Resets a buffer with a callback block.

