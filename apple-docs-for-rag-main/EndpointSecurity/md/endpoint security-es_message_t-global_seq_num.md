

- Endpoint Security
- es_message_t
-  global_seq_num 

Instance Property

# global_seq_num

The global sequence number of the message.

Mac CatalystmacOS

``` source
var global_seq_num: UInt64
```

## Discussion

Inspect the global sequence number per-client to detect whether the kernel had to drop events for this client. If the kernel doesn’t drop any events for this client, `global_seq_num` increments by 1 for every message.

To determine whether the kernel dropped events, compare the previous value of `global_seq_num` to the value received in the latest message. When the kernel drops no events, the difference is 1, since the current message increments the counter. You can therefore calculate the number of dropped messages as follows:

```
numberOfDroppedEvents = thisMessage.global_seq_num - (prevMessage.global_seq_num + 1)
```

Dropped events generally indicate that the kernel generated more events than the client could handle.

This field is available if the message version is greater than `4`.

Tip

For an equivalent counter that filters by client and event type, see seq_num.

## See Also

### Inspecting Timing Properties

var time: timespec

The time the event occurred, expressed as a Darwin time value.

var mach_time: UInt64

The time the event occurred, as a Mach time value.

var deadline: UInt64

The deadline by which your app must respond to the event.

var seq_num: UInt64

The sequence number of the message.

