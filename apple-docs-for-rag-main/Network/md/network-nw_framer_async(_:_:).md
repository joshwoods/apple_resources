

- Network
-  nw_framer_async(\_:\_:) 

Function

# nw_framer_async(\_:\_:)

Requests that a block be executed on the connection’s internal scheduling context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func nw_framer_async(
    _ framer: nw_framer_t,
    _ async_block: @escaping nw_framer_block_t
)
```

## Discussion

You should call this if you need to call any framer functions but are in another scheduling context.

## See Also

### Handling Asynchronous Events

func nw_framer_schedule_wakeup(nw_framer_t, UInt64)

Requests that the nw_framer_wakeup_handler_t be called on your protocol at a specific time in the future.

var NW_FRAMER_WAKEUP_TIME_FOREVER: UInt64

A sentinel value that indicates that no wakeup should be delivered.

func nw_framer_set_wakeup_handler(nw_framer_t, nw_framer_wakeup_handler_t)

Sets a handler to receive scheduled wakeup events.

typealias nw_framer_wakeup_handler_t

A handler that delivers a scheduled wakeup event.

typealias nw_framer_block_t

A block to be invoked asynchronously on your framer protocol’s scheduling context.

