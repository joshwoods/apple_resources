

- Security
-  sec_protocol_metadata_get_negotiated_protocol_version(\_:) Deprecated

Function

# sec_protocol_metadata_get_negotiated_protocol_version(\_:)

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.14–10.15DeprecatedtvOS 12.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 5.0–6.0Deprecated

``` source
func sec_protocol_metadata_get_negotiated_protocol_version(_ metadata: sec_protocol_metadata_t) -> SSLProtocol
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

## Return Value

A SSLProtocol enum of the TLS version.

## Discussion

```
  Get the negotiated TLS version.
```

