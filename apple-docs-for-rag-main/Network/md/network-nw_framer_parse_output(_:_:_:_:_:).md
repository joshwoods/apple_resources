

- Network
-  nw_framer_parse_output(\_:\_:\_:\_:\_:) 

Function

# nw_framer_parse_output(\_:\_:\_:\_:\_:)

Examines the content of output data while inside your output handler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func nw_framer_parse_output(
    _ framer: nw_framer_t,
    _ minimum_incomplete_length: Int,
    _ maximum_length: Int,
    _ temp_buffer: UnsafeMutablePointer?,
    _ parse: (UnsafeMutablePointer?, Int, Bool) -> Int
) -> Bool
```

## Parameters 

`framer`  

A network framer instance.

`minimum_incomplete_length`  

The minimum number of bytes that should be delivered to the parse completion.

`maximum_length`  

The maximum number of bytes that should be delivered to the parse completion.

`temp_buffer`  

An optional buffer into which the parser will copy bytes. Use this if you need to make guarantees about byte alignment.

`parse`  

A completion handler that will be called inline to examine a region of bytes.

## Return Value

Returns true if the requested length was available to parse, or false if the conditions could not be met.

## See Also

### Handling Output Data

func nw_framer_set_output_handler(nw_framer_t, nw_framer_output_handler_t)

Sets a block to handle new outbound messages.

typealias nw_framer_output_handler_t

A handler that notifies your protocol about a new outbound message.

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

