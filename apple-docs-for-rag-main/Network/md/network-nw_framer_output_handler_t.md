

- Network
-  nw_framer_output_handler_t 

Type Alias

# nw_framer_output_handler_t

A handler that notifies your protocol about a new outbound message.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_framer_output_handler_t = (nw_framer_t, nw_framer_message_t, Int, Bool) -> Void
```

## Parameters 

`framer`  

The framer instance associated with the connection.

`message`  

The framer message passed by the application.

`message_length`  

The length of the message content being sent.

`is_complete`  

A boolean indicating if this the last chunk of a message.

## Discussion

The output handler is your opportunity to encapsulate or encode a signle application message. You should write any output using nw_framer_write_output(_:_:_:), nw_framer_write_output_data(_:_:), or nw_framer_write_output_no_copy(_:_:) before returning from the output handler. If you do not write a message, the application message will be discarded.

## See Also

### Handling Output Data

func nw_framer_set_output_handler(nw_framer_t, nw_framer_output_handler_t)

Sets a block to handle new outbound messages.

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

