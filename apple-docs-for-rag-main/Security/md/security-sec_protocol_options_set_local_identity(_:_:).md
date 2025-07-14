

- Security
-  sec_protocol_options_set_local_identity(\_:\_:) 

Function

# sec_protocol_options_set_local_identity(\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_options_set_local_identity(
    _ options: sec_protocol_options_t,
    _ identity: sec_identity_t
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`identity`  

A `sec_identity_t` instance carrying the private key and certificate.

## Discussion

```
  Set the local identity to be used for this protocol instance.
```

