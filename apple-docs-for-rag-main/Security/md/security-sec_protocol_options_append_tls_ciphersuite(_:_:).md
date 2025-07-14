

- Security
-  sec_protocol_options_append_tls_ciphersuite(\_:\_:) 

Function

# sec_protocol_options_append_tls_ciphersuite(\_:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sec_protocol_options_append_tls_ciphersuite(
    _ options: sec_protocol_options_t,
    _ ciphersuite: tls_ciphersuite_t
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`ciphersuite`  

A `tls_ciphersuite_t` value.

## Discussion

```
  Append a TLS ciphersuite to the set of enabled ciphersuites.
```

