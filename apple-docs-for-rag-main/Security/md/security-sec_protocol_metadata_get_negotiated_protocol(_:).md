

- Security
-  sec_protocol_metadata_get_negotiated_protocol(\_:) 

Function

# sec_protocol_metadata_get_negotiated_protocol(\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_metadata_get_negotiated_protocol(_ metadata: sec_protocol_metadata_t) -> UnsafePointer?
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

## Return Value

A NULL-terminated string carrying the negotiated protocol.

## Discussion

```
  Get the application protocol negotiated, e.g., via the TLS ALPN extension.
```

