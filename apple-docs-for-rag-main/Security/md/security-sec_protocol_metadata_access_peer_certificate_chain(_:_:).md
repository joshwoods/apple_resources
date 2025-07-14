

- Security
-  sec_protocol_metadata_access_peer_certificate_chain(\_:\_:) 

Function

# sec_protocol_metadata_access_peer_certificate_chain(\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_metadata_access_peer_certificate_chain(
    _ metadata: sec_protocol_metadata_t,
    _ handler: @escaping (sec_certificate_t) -> Void
) -> Bool
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

`handler`  

A block to invoke one or more times with sec_certificate_t objects

## Return Value

Returns true if the peer certificates were accessible, false otherwise.

## Discussion

```
  Get the certificate chain of the protocol instance peer.
```

