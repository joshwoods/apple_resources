

- Endpoint Security
- es_message_t
-  deadline 

Instance Property

# deadline

The deadline by which your app must respond to the event.

Mac CatalystmacOS

``` source
var deadline: UInt64
```

## Discussion

If you fail to respond to an event before this deadline, Endpoint Security may terminate the client process, or restart the process if it’s a system extension. If your client repeatedly misses deadlines, Endpoint Security may refuse new connections from es_new_client(_:_:) altogether.

## See Also

### Inspecting Timing Properties

var time: timespec

The time the event occurred, expressed as a Darwin time value.

var mach_time: UInt64

The time the event occurred, as a Mach time value.

var seq_num: UInt64

The sequence number of the message.

var global_seq_num: UInt64

The global sequence number of the message.

