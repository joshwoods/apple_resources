

- Endpoint Security
-  es_proc_suspend_resume_type_t 

Structure

# es_proc_suspend_resume_type_t

The type of a process suspension or resumption event.

Mac CatalystmacOS

``` source
struct es_proc_suspend_resume_type_t
```

## Topics

### Event Types

var ES_PROC_SUSPEND_RESUME_TYPE_SUSPEND: es_proc_suspend_resume_type_t

An event type for process suspension events.

var ES_PROC_SUSPEND_RESUME_TYPE_RESUME: es_proc_suspend_resume_type_t

An event type for process resumption events.

var ES_PROC_SUSPEND_RESUME_TYPE_SHUTDOWN_SOCKETS: es_proc_suspend_resume_type_t

An event type for process socket shutdown events.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>?

The process targeted by this event.

var type: es_proc_suspend_resume_type_t

The type of event: suspend, resume, or socket shutdown.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

