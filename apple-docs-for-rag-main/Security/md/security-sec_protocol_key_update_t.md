

- Security
-  sec_protocol_key_update_t 

Type Alias

# sec_protocol_key_update_t

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias sec_protocol_key_update_t = (sec_protocol_metadata_t, @escaping sec_protocol_key_update_complete_t) -> Void
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

`complete`  

A `sec_protocol_key_update_complete_t` to be invoked when the key update is complete.

## Discussion

```
  Block to be invoked when the protocol key MUST be updated.
```

