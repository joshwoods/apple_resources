

- Endpoint Security
-  es_proc_check_type_t 

Structure

# es_proc_check_type_t

The type of call used when a process checks on the access of the target process.

Mac CatalystmacOS

``` source
struct es_proc_check_type_t
```

## Overview

This value provides detail, in coordination with flavor from es_event_proc_check_t, to identify the functions and the type of data returned from checks called in `libproc.h`.

## Topics

### Process Check Result Types

var ES_PROC_CHECK_TYPE_DIRTYCONTROL: es_proc_check_type_t

A type of process check that uses the process’s dirty state.

var ES_PROC_CHECK_TYPE_LISTPIDS: es_proc_check_type_t

A type of process check that lists related process identifiers.

var ES_PROC_CHECK_TYPE_PIDFDINFO: es_proc_check_type_t

A type of process check that gets file descriptor information.

var ES_PROC_CHECK_TYPE_PIDFILEPORTINFO: es_proc_check_type_t

A type of process check that gets port information.

var ES_PROC_CHECK_TYPE_PIDINFO: es_proc_check_type_t

A type of process check that gets basic process information.

var ES_PROC_CHECK_TYPE_PIDRUSAGE: es_proc_check_type_t

A type of process check that gets a process’s resource usage information.

var ES_PROC_CHECK_TYPE_SETCONTROL: es_proc_check_type_t

A type of process check that sets the process control state.

### Deprecated Result Types

var ES_PROC_CHECK_TYPE_KERNMSGBUF: es_proc_check_type_t

A type of process check that checks the message buffer.

Deprecated

var ES_PROC_CHECK_TYPE_TERMINATE: es_proc_check_type_t

A type of process check that terninates a process.

Deprecated

var ES_PROC_CHECK_TYPE_UDATA_INFO: es_proc_check_type_t

A type of process check that involves a user data token.

Deprecated

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

var flavor: Int32

A representation of the information sought by a process based on the type member of es_event_proc_check_t.

var target: UnsafeMutablePointer&lt;es_process_t>?

The process targeted by this event.

var type: es_proc_check_type_t

The type of call number used to check the access on the target process.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

