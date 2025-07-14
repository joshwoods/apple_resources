

- Security
-  sec_protocol_options_append_tls_ciphersuite_group(\_:\_:) 

Function

# sec_protocol_options_append_tls_ciphersuite_group(\_:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sec_protocol_options_append_tls_ciphersuite_group(
    _ options: sec_protocol_options_t,
    _ group: tls_ciphersuite_group_t
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`group`  

A tls_ciphersuite_group_t value.

## Discussion

```
  Append a TLS ciphersuite group to the set of enabled ciphersuites.
```

