

- Security
-  sec_protocol_options_set_min_tls_protocol_version(\_:\_:) 

Function

# sec_protocol_options_set_min_tls_protocol_version(\_:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sec_protocol_options_set_min_tls_protocol_version(
    _ options: sec_protocol_options_t,
    _ version: tls_protocol_version_t
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`version`  

A tls_protocol_version_t enum value.

## Discussion

```
  Set the minimum support TLS version.
```

