

- Network
-  nw_framer_set_output_handler(\_:\_:) 

Function

# nw_framer_set_output_handler(\_:\_:)

Sets a block to handle new outbound messages.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func nw_framer_set_output_handler(
    _ framer: nw_framer_t,
    _ output_handler: @escaping nw_framer_output_handler_t
)
```

## See Also

### Handling Output Data

typealias nw_framer_output_handler_t

A handler that notifies your protocol about a new outbound message.

func nw_framer_parse_output(nw_framer_t, Int, Int, UnsafeMutablePointer&lt;UInt8>?, (UnsafeMutablePointer&lt;UInt8>?, Int, Bool) -> Int) -> Bool

Examines the content of output data while inside your output handler.

typealias nw_framer_parse_completion_t

A handler that examines a range of data being sent or received.

func nw_framer_write_output(nw_framer_t, UnsafePointer&lt;UInt8>, Int)

Sends arbitrary output data in a buffer from your protocol to the next protocol.

func nw_framer_write_output_data(nw_framer_t, dispatch_data_t)

Sends arbitrary output data from your protocol to the next protocol.

func nw_framer_write_output_no_copy(nw_framer_t, Int) -> Bool

Sends a specific number of bytes from a message while inside your output handler.

func nw_framer_pass_through_output(nw_framer_t)

Indicates that your protocol no longer needs to handle output data.

