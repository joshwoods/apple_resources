

- Network
-  nw_framer_input_handler_t 

Type Alias

# nw_framer_input_handler_t

A handler that notifies your protocol that new inbound data is available to parse.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_framer_input_handler_t = (nw_framer_t) -> Int
```

## See Also

### Handling Input Data

func nw_framer_set_input_handler(nw_framer_t, nw_framer_input_handler_t)

Sets a block to handle new inbound data.

func nw_framer_parse_input(nw_framer_t, Int, Int, UnsafeMutablePointer&lt;UInt8>?, (UnsafeMutablePointer&lt;UInt8>?, Int, Bool) -> Int) -> Bool

Examines the content of input data while inside your input handler block.

typealias nw_framer_parse_completion_t

A handler that examines a range of data being sent or received.

func nw_framer_deliver_input(nw_framer_t, UnsafePointer&lt;UInt8>, Int, nw_framer_message_t, Bool)

Delivers an inbound message containing arbitrary data from your protocol to the application.

func nw_framer_deliver_input_no_copy(nw_framer_t, Int, nw_framer_message_t, Bool) -> Bool

Delivers an inbound message containing a specific number of next received bytes.

func nw_framer_pass_through_input(nw_framer_t)

Indicates that your protocol no longer needs to handle input data.

