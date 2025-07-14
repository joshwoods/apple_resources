

- Endpoint Security
-  es_event_proc_suspend_resume_t 

Structure

# es_event_proc_suspend_resume_t

A type for an event that indicates a call to suspend, resume, or shut down sockets for a process.

Mac CatalystmacOS

``` source
struct es_event_proc_suspend_resume_t
```

## Topics

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>?

The process targeted by this event.

var type: es_proc_suspend_resume_type_t

The type of event: suspend, resume, or socket shutdown.

struct es_proc_suspend_resume_type_t

The type of a process suspension or resumption event.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init()

init(target: UnsafeMutablePointer&lt;es_process_t>?, type: es_proc_suspend_resume_type_t, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Interprocess Events

struct es_event_trace_t

A type for an event that indicates an attempt by one process to attach to another process.

struct es_event_remote_thread_create_t

A type for an event that indicates an attempt by one process to create a thread in another process.

