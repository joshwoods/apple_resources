

- Security
-  sec_protocol_options_set_challenge_block(\_:\_:\_:) 

Function

# sec_protocol_options_set_challenge_block(\_:\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_options_set_challenge_block(
    _ options: sec_protocol_options_t,
    _ challenge_block: @escaping sec_protocol_challenge_t,
    _ challenge_queue: dispatch_queue_t
)
```

## Parameters 

`options`  

A `sec_protocol_options_t` instance.

## Discussion

```
  Set the challenge block.
```

```
  A `sec_protocol_challenge_t` block.
```

```
  A `dispatch_queue_t` on which the challenge block should be called.
```

