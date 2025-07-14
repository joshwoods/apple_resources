

- Network
-  nw_framer_create_options(\_:) 

Function

# nw_framer_create_options(\_:)

Initializes a set of protocol options with a custom framer definition.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func nw_framer_create_options(_ framer_definition: nw_protocol_definition_t) -> nw_protocol_options_t
```

## See Also

### Adding Framers to Connections

func nw_framer_create_definition(UnsafePointer&lt;CChar>, UInt32, nw_framer_start_handler_t) -> nw_protocol_definition_t

Initializes a new protocol definition based on your protocol implementation.

typealias nw_framer_start_handler_t

A handler that represents the entry point into your custom protocol.

typealias nw_framer_t

An object that represents a single instance of your custom protocol running in a connection.

struct nw_framer_start_result_t

Results that you send to indicate the disposition of your protocol after the start handler is invoked.

var NW_FRAMER_CREATE_FLAGS_DEFAULT: Int32

A constant flag value that indicates that the default framer protocol behavior should be used.

