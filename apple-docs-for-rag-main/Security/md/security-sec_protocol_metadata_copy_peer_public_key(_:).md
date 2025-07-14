

- Security
-  sec_protocol_metadata_copy_peer_public_key(\_:) 

Function

# sec_protocol_metadata_copy_peer_public_key(\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_metadata_copy_peer_public_key(_ metadata: sec_protocol_metadata_t) -> dispatch_data_t?
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

## Return Value

A `dispatch_data_t` containing the peer’s raw public key.

## Discussion

```
  Get the protocol instance peer's public key.
```

