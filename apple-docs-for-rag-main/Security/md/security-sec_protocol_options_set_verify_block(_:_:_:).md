

- Security
-  sec_protocol_options_set_verify_block(\_:\_:\_:) 

Function

# sec_protocol_options_set_verify_block(\_:\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_options_set_verify_block(
    _ options: sec_protocol_options_t,
    _ verify_block: @escaping sec_protocol_verify_t,
    _ verify_block_queue: dispatch_queue_t
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

## Discussion

```
  Set the verify block.
```

```
  A `sec_protocol_verify_t` block.
```

```
  A `dispatch_queue_t` on which the verify block should be called.
```

