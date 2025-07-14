

- Endpoint Security
- es_message_t
-  time 

Instance Property

# time

The time the event occurred, expressed as a Darwin time value.

Mac CatalystmacOS

``` source
var time: timespec
```

## See Also

### Inspecting Timing Properties

var mach_time: UInt64

The time the event occurred, as a Mach time value.

var deadline: UInt64

The deadline by which your app must respond to the event.

var seq_num: UInt64

The sequence number of the message.

var global_seq_num: UInt64

The global sequence number of the message.

