

- Core Media
- CMBufferQueue
-  reset(\_:) 

Instance Method

# reset(\_:)

Resets a buffer with a callback block.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func reset(_ body: (CMBuffer) throws -> ()) throws
```

## Parameters 

`body`  

## See Also

### Managing a Queue

func enqueue(CMBuffer) throws

Enqueues a buffer to the queue.

func dequeue() -> CMBuffer?

Dequeues a buffer from the queue.

func dequeueIfDataReady() -> CMBuffer?

Dequeues a buffer from the queue, if it’s ready.

func markEndOfData() throws

Marks a buffer as being at the end of its data.

func reset() throws

Empties the queue and resets its end-of-data state.

