

- Security
-  sec_protocol_options_set_peer_authentication_required(\_:\_:) 

Function

# sec_protocol_options_set_peer_authentication_required(\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_options_set_peer_authentication_required(
    _ options: sec_protocol_options_t,
    _ peer_authentication_required: Bool
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`peer_authentication_required`  

Flag to enable or disable mandatory peer authentication.

## Discussion

```
  Enable or disable peer authentication. Clients default to true, whereas servers default to false.
```

