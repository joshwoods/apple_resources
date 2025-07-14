

- Endpoint Security
- es_event_file_provider_materialize_t
-  instigator_token 

Instance Property

# instigator_token

Mac CatalystmacOS

``` source
var instigator_token: audit_token_t
```

## See Also

### Inspecting Event Properties

var instigator: UnsafeMutablePointer&lt;es_process_t>?

The process that instigated the event.

var source: UnsafeMutablePointer&lt;es_file_t>

The source file.

var target: UnsafeMutablePointer&lt;es_file_t>

The target fle.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

