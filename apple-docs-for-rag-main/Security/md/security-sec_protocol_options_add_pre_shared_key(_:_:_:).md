

- Security
-  sec_protocol_options_add_pre_shared_key(\_:\_:\_:) 

Function

# sec_protocol_options_add_pre_shared_key(\_:\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_options_add_pre_shared_key(
    _ options: sec_protocol_options_t,
    _ psk: dispatch_data_t,
    _ psk_identity: dispatch_data_t
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

`psk`  

A dispatch_data_t containing a PSK blob.

`psk_identity`  

A dispatch_data_t containing a PSK identity blob.

## Discussion

```
  Add a pre-shared key (PSK) and its identity to the options.
```

