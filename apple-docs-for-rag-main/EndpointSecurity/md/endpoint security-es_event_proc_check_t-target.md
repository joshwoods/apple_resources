

- Endpoint Security
- es_event_proc_check_t
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

var flavor: Int32

A representation of the information sought by a process based on the type member of es_event_proc_check_t.

var type: es_proc_check_type_t

The type of call number used to check the access on the target process.

struct es_proc_check_type_t

The type of call used when a process checks on the access of the target process.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

