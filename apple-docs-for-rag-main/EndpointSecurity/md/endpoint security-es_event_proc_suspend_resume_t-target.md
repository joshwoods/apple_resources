

- Endpoint Security
- es_event_proc_suspend_resume_t
-  target 

Instance Property

# target

The process targeted by this event.

Mac CatalystmacOS

``` source
var target: UnsafeMutablePointer?
```

## See Also

### Inspecting Event Properties

var type: es_proc_suspend_resume_type_t

The type of event: suspend, resume, or socket shutdown.

struct es_proc_suspend_resume_type_t

The type of a process suspension or resumption event.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

