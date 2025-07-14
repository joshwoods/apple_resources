

- Endpoint Security
- es_message_t
-  thread 

Instance Property

# thread

The thread that took the action defined in a message.

Mac CatalystmacOS

``` source
var thread: UnsafeMutablePointer?
```

## Discussion

This field may be NULL when threading doesn’t apply. This includes trace events that describe calls to `ptrace(PT_TRACE_ME`) or code-signing invalidation events resulting from another process calling `csops(CS_OPS_MARKINVALID)`.

## See Also

### Inspecting Thread Properties

struct es_thread_t

A structure that represents a thread in a process.

