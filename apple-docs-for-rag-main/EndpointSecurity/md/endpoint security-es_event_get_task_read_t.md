

- Endpoint Security
-  es_event_get_task_read_t 

Structure

# es_event_get_task_read_t

A type for an event that indicates the retrieval of a task’s read port.

Mac CatalystmacOS

``` source
struct es_event_get_task_read_t
```

## Overview

This event represents a process that obtains a send right to a task read port, through `SYS_task_read_for_pid` or functions like `task_identity_token_get_task_port(_:_:_:)`.

Note

For more information on ports and port rights, see the “Ports, Port Rights, Port Sets, and Port Namespaces” section of Mach Overview in the Kernel Programming Guide.

## Topics

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>

The process targeted by this event.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(target: UnsafeMutablePointer&lt;es_process_t>, type: es_get_task_type_t, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

### Instance Properties

var type: es_get_task_type_t

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Task Port Event Types

struct es_event_get_task_t

A type for an event that indicates the retrieval of a task’s control port.

struct es_event_get_task_inspect_t

A type for an event that indicates the retrieval of a task’s inspect port.

struct es_event_get_task_name_t

A type for an event that indicates the retrieval of a task’s name port.

