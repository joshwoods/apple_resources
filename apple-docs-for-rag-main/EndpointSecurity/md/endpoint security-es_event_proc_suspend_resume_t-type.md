

- Endpoint Security
- es_event_proc_suspend_resume_t
-  type 

Instance Property

# type

The type of event: suspend, resume, or socket shutdown.

Mac CatalystmacOS

``` source
var type: es_proc_suspend_resume_type_t
```

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>?

The process targeted by this event.

struct es_proc_suspend_resume_type_t

The type of a process suspension or resumption event.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

