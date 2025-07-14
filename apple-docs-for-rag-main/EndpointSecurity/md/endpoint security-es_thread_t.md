

- Endpoint Security
-  es_thread_t 

Structure

# es_thread_t

A structure that represents a thread in a process.

Mac CatalystmacOS

``` source
struct es_thread_t
```

## Topics

### Identifying the Thread

var thread_id: UInt64

The unique identifier of the thread.

### Initializers

init()

init(thread_id: UInt64)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Inspecting Thread Properties

var thread: UnsafeMutablePointer&lt;es_thread_t>?

The thread that took the action defined in a message.

