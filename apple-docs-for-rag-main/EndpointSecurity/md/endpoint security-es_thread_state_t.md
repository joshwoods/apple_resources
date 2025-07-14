

- Endpoint Security
-  es_thread_state_t 

Structure

# es_thread_state_t

A description of a thread’s machine-specfiic state.

Mac CatalystmacOS

``` source
struct es_thread_state_t
```

## Overview

To work with thread state, see the definitions in the include file `mach/thread_status.h` and corresponding machine-dependent headers.

## Topics

### Inspecting Thread State

var flavor: Int32

An indication of the representation of the machine-specific thread state.

var state: es_token_t

The machine-specific thread state.

struct es_token_t

An arbitrary buffer of data with its size.

### Initializers

init()

init(flavor: Int32, state: es_token_t)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>

The process targeted to spawn a new thread.

var thread_state: UnsafeMutablePointer&lt;es_thread_state_t>?

The new thread’s state.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

