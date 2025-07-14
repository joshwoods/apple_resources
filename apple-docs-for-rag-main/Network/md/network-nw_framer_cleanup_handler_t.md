

- Network
-  nw_framer_cleanup_handler_t 

Type Alias

# nw_framer_cleanup_handler_t

A handler that tells your protocol to clean up all allocations before being deallocated.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_framer_cleanup_handler_t = (nw_framer_t) -> Void
```

## See Also

### Managing Instance Lifetime

func nw_framer_mark_ready(nw_framer_t)

Indicates to a connection that your protocol’s handshake is complete.

func nw_framer_mark_failed_with_error(nw_framer_t, Int32)

Indicates to a connection that your protocol has encountered an error, or has gracefully closed.

func nw_framer_prepend_application_protocol(nw_framer_t, nw_protocol_options_t) -> Bool

Dynamically adds another protocol that will run above your protocol after your protocol calls nw_framer_mark_ready(_:).

func nw_framer_set_stop_handler(nw_framer_t, nw_framer_stop_handler_t)

Sets a block to handle when the connection is being closed.

typealias nw_framer_stop_handler_t

A handler that requests that your protocol send any final messages to close the connection.

func nw_framer_set_cleanup_handler(nw_framer_t, nw_framer_cleanup_handler_t)

Sets a block to handle the final cleanup of allocations made by your protocol instance.

