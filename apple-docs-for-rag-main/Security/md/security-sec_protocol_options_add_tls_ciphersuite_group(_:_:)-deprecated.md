

- Security
-  sec_protocol_options_add_tls_ciphersuite_group(\_:\_:) Deprecated

Function

# sec_protocol_options_add_tls_ciphersuite_group(\_:\_:)

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 12.0–13.0DeprecatedmacOS 10.14–10.15DeprecatedtvOS 12.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 5.0–6.0Deprecated

``` source
func sec_protocol_options_add_tls_ciphersuite_group(
    _ options: sec_protocol_options_t,
    _ group: SSLCiphersuiteGroup
)
```

Deprecated

Use sec_protocol_options_append_tls_ciphersuite_group

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`group`  

A SSLCipherSuiteGroup value.

## Discussion

```
  Add a TLS ciphersuite group to the set of enabled ciphersuites.
```

