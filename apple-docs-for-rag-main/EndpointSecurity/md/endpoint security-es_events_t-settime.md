

- Endpoint Security
- es_events_t
-  settime 

Instance Property

# settime

Properties of an event that indicates the modification of the system time.

Mac CatalystmacOS

``` source
var settime: es_event_settime_t { get set }
```

## Discussion

The system won’t fire this event if the source app contains the entitlement `com.apple.private.settime`.

Even if an Endpoint Security client responds to an ES_EVENT_TYPE_AUTH_SETTIME event with ES_AUTH_RESULT_ALLOW, the operation may still fail. For example, the process setting the time may lack sufficient privileges.

