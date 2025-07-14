

- Endpoint Security
- es_event_proc_suspend_resume_t
-  reserved 

Instance Property

# reserved

An unused field reserved for future use.

Mac CatalystmacOS

``` source
var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)
```

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>?

The process targeted by this event.

var type: es_proc_suspend_resume_type_t

The type of event: suspend, resume, or socket shutdown.

struct es_proc_suspend_resume_type_t

The type of a process suspension or resumption event.

