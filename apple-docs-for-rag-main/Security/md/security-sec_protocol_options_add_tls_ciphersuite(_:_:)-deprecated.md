

- Security
-  sec_protocol_options_add_tls_ciphersuite(\_:\_:) Deprecated

Function

# sec_protocol_options_add_tls_ciphersuite(\_:\_:)

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 12.0–13.0DeprecatedmacOS 10.14–10.15DeprecatedtvOS 12.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 5.0–6.0Deprecated

``` source
func sec_protocol_options_add_tls_ciphersuite(
    _ options: sec_protocol_options_t,
    _ ciphersuite: SSLCipherSuite
)
```

Deprecated

Use sec_protocol_options_append_tls_ciphersuite

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`ciphersuite`  

A SSLCipherSuite value.

## Discussion

```
  Add a TLS ciphersuite to the set of enabled ciphersuites.
```

