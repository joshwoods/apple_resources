

- Network
-  nw_framer_start_handler_t 

Type Alias

# nw_framer_start_handler_t

A handler that represents the entry point into your custom protocol.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_framer_start_handler_t = (nw_framer_t) -> nw_framer_start_result_t
```

## Return Value

Return a start result indicating if the connection should become ready immediately, or wait for you protocol to perform a handshake.

## Discussion

Within your start handler, you should register all other callbacks for your custom protocol, particularly nw_framer_set_output_handler(_:_:) and nw_framer_set_input_handler(_:_:).

Any state that you need to be associated with your protocol as customizable options can be captured within the start block.

## See Also

### Adding Framers to Connections

func nw_framer_create_definition(UnsafePointer&lt;CChar>, UInt32, nw_framer_start_handler_t) -> nw_protocol_definition_t

Initializes a new protocol definition based on your protocol implementation.

typealias nw_framer_t

An object that represents a single instance of your custom protocol running in a connection.

struct nw_framer_start_result_t

Results that you send to indicate the disposition of your protocol after the start handler is invoked.

var NW_FRAMER_CREATE_FLAGS_DEFAULT: Int32

A constant flag value that indicates that the default framer protocol behavior should be used.

func nw_framer_create_options(nw_protocol_definition_t) -> nw_protocol_options_t

Initializes a set of protocol options with a custom framer definition.

