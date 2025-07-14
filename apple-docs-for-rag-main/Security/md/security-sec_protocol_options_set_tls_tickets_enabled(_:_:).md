

- Security
-  sec_protocol_options_set_tls_tickets_enabled(\_:\_:) 

Function

# sec_protocol_options_set_tls_tickets_enabled(\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_options_set_tls_tickets_enabled(
    _ options: sec_protocol_options_t,
    _ tickets_enabled: Bool
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`tickets_enabled`  

Flag to enable or disable TLS session ticket support.

## Discussion

```
  Enable or disable TLS session ticket support.
```

