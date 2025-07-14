

- Endpoint Security
- es_event_file_provider_materialize_t
-  reserved 

Instance Property

# reserved

An unused field reserved for future use.

Mac CatalystmacOS

``` source
var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)
```

## See Also

### Inspecting Event Properties

var instigator: UnsafeMutablePointer&lt;es_process_t>?

The process that instigated the event.

var instigator_token: audit_token_t

var source: UnsafeMutablePointer&lt;es_file_t>

The source file.

var target: UnsafeMutablePointer&lt;es_file_t>

The target fle.

