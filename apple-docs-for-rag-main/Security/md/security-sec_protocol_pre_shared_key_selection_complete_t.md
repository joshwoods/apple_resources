

- Security
-  sec_protocol_pre_shared_key_selection_complete_t 

Type Alias

# sec_protocol_pre_shared_key_selection_complete_t

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias sec_protocol_pre_shared_key_selection_complete_t = (dispatch_data_t?) -> Void
```

## Parameters 

`psk_identity`  

A `dispatch_data_t` instance carrying the chosen PSK identity, or nil if one does not match.

## Discussion

```
  Block to be invoked when a PSK selection event is complete and a PSK identity is chosen.
```

