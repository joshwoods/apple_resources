

- Security
-  sec_protocol_options_set_tls_diffie_hellman_parameters(\_:\_:) Deprecated

Function

# sec_protocol_options_set_tls_diffie_hellman_parameters(\_:\_:)

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.14–10.15DeprecatedtvOS 12.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 5.0–6.0Deprecated

``` source
func sec_protocol_options_set_tls_diffie_hellman_parameters(
    _ options: sec_protocol_options_t,
    _ params: dispatch_data_t
)
```

Deprecated

DHE ciphersuites are no longer supported

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`params`  

A dispatch_data_t containing legacy Diffie-Hellman parameters.

## Discussion

```
  Set the supported Diffie-Hellman parameters.
```

