

- Endpoint Security
-  es_event_remote_thread_create_t 

Structure

# es_event_remote_thread_create_t

A type for an event that indicates an attempt by one process to create a thread in another process.

Mac CatalystmacOS

``` source
struct es_event_remote_thread_create_t
```

## Topics

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>

The process targeted to spawn a new thread.

var thread_state: UnsafeMutablePointer&lt;es_thread_state_t>?

The new thread’s state.

struct es_thread_state_t

A description of a thread’s machine-specfiic state.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(target: UnsafeMutablePointer&lt;es_process_t>, thread_state: UnsafeMutablePointer&lt;es_thread_state_t>?, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Interprocess Events

struct es_event_proc_suspend_resume_t

A type for an event that indicates a call to suspend, resume, or shut down sockets for a process.

struct es_event_trace_t

A type for an event that indicates an attempt by one process to attach to another process.

