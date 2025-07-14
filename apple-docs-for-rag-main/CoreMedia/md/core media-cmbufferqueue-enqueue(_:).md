

- Core Media
- CMBufferQueue
-  enqueue(\_:) 

Instance Method

# enqueue(\_:)

Enqueues a buffer to the queue.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func enqueue(_ buffer: CMBuffer) throws
```

## Parameters 

`buffer`  

The buffer to enqueue.

## See Also

### Managing a Queue

func dequeue() -> CMBuffer?

Dequeues a buffer from the queue.

func dequeueIfDataReady() -> CMBuffer?

Dequeues a buffer from the queue, if it’s ready.

func markEndOfData() throws

Marks a buffer as being at the end of its data.

func reset() throws

Empties the queue and resets its end-of-data state.

func reset((CMBuffer) throws -> ()) throws

Resets a buffer with a callback block.

