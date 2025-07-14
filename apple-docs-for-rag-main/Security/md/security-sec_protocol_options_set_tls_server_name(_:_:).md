

- Security
-  sec_protocol_options_set_tls_server_name(\_:\_:) 

Function

# sec_protocol_options_set_tls_server_name(\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_options_set_tls_server_name(
    _ options: sec_protocol_options_t,
    _ server_name: UnsafePointer
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`server_name`  

A NULL-terminated string carrying the server name.

## Discussion

```
  Set the server name to be used when verifying the peer's certificate. This will override
  the server name obtained from the endpoint.
```

