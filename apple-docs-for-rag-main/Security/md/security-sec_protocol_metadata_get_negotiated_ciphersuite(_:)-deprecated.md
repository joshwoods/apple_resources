

- Security
-  sec_protocol_metadata_get_negotiated_ciphersuite(\_:) Deprecated

Function

# sec_protocol_metadata_get_negotiated_ciphersuite(\_:)

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 12.0–13.0DeprecatedmacOS 10.14–10.15DeprecatedtvOS 12.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 5.0–6.0Deprecated

``` source
func sec_protocol_metadata_get_negotiated_ciphersuite(_ metadata: sec_protocol_metadata_t) -> SSLCipherSuite
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

## Return Value

A SSLCipherSuite.

## Discussion

```
  Get the negotiated TLS ciphersuite.
```

