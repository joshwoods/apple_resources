

- Security
-  sec_protocol_verify_t 

Type Alias

# sec_protocol_verify_t

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias sec_protocol_verify_t = (sec_protocol_metadata_t, sec_trust_t, @escaping sec_protocol_verify_complete_t) -> Void
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

`trust_ref`  

A `sec_trust_t` instance.

`complete`  

A `sec_protocol_verify_finish_t` to be invoked when verification is complete.

## Discussion

```
  Block to be invoked when the protocol instance must verify the peer.

  NOTE: this may be called one or more times for a given connection.
```

