

- Network
-  nw_framer_wakeup_handler_t 

Type Alias

# nw_framer_wakeup_handler_t

A handler that delivers a scheduled wakeup event.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_framer_wakeup_handler_t = (nw_framer_t) -> Void
```

## See Also

### Handling Asynchronous Events

func nw_framer_schedule_wakeup(nw_framer_t, UInt64)

Requests that the nw_framer_wakeup_handler_t be called on your protocol at a specific time in the future.

var NW_FRAMER_WAKEUP_TIME_FOREVER: UInt64

A sentinel value that indicates that no wakeup should be delivered.

func nw_framer_set_wakeup_handler(nw_framer_t, nw_framer_wakeup_handler_t)

Sets a handler to receive scheduled wakeup events.

func nw_framer_async(nw_framer_t, nw_framer_block_t)

Requests that a block be executed on the connection’s internal scheduling context.

typealias nw_framer_block_t

A block to be invoked asynchronously on your framer protocol’s scheduling context.

