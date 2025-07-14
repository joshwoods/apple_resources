

- Endpoint Security
-  es_event_file_provider_materialize_t 

Structure

# es_event_file_provider_materialize_t

A type for an event that indicates the materialization of a file provider.

Mac CatalystmacOS

``` source
struct es_event_file_provider_materialize_t
```

## Topics

### Inspecting Event Properties

var instigator: UnsafeMutablePointer&lt;es_process_t>?

The process that instigated the event.

var instigator_token: audit_token_t

var source: UnsafeMutablePointer&lt;es_file_t>

The source file.

var target: UnsafeMutablePointer&lt;es_file_t>

The target fle.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(instigator: UnsafeMutablePointer&lt;es_process_t>?, source: UnsafeMutablePointer&lt;es_file_t>, target: UnsafeMutablePointer&lt;es_file_t>, instigator_token: audit_token_t, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### File Provider Event Types

struct es_event_file_provider_update_t

A type for an event that indicates an update to a file provider.

