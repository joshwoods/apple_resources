

- Security
-  sec_protocol_options_set_tls_max_version(\_:\_:) Deprecated

Function

# sec_protocol_options_set_tls_max_version(\_:\_:)

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 12.0–13.0DeprecatedmacOS 10.14–10.15DeprecatedtvOS 12.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 5.0–6.0Deprecated

``` source
func sec_protocol_options_set_tls_max_version(
    _ options: sec_protocol_options_t,
    _ version: SSLProtocol
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`version`  

A SSLProtocol enum value.

## Discussion

```
  Set the maximum support TLS version.
```

