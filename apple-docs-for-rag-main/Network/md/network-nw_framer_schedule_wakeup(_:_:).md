

- Network
-  nw_framer_schedule_wakeup(\_:\_:) 

Function

# nw_framer_schedule_wakeup(\_:\_:)

Requests that the nw_framer_wakeup_handler_t be called on your protocol at a specific time in the future.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func nw_framer_schedule_wakeup(
    _ framer: nw_framer_t,
    _ milliseconds: UInt64
)
```

## See Also

### Handling Asynchronous Events

var NW_FRAMER_WAKEUP_TIME_FOREVER: UInt64

A sentinel value that indicates that no wakeup should be delivered.

func nw_framer_set_wakeup_handler(nw_framer_t, nw_framer_wakeup_handler_t)

Sets a handler to receive scheduled wakeup events.

typealias nw_framer_wakeup_handler_t

A handler that delivers a scheduled wakeup event.

func nw_framer_async(nw_framer_t, nw_framer_block_t)

Requests that a block be executed on the connection’s internal scheduling context.

typealias nw_framer_block_t

A block to be invoked asynchronously on your framer protocol’s scheduling context.

