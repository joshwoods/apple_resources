

- Core Services
- File System Events
-  FSEventStreamEventId 

Type Alias

# FSEventStreamEventId

Mac Catalyst 13.0+macOS 10.5+

``` source
typealias FSEventStreamEventId = UInt64
```

## Discussion

Event IDs that can be passed to the FSEventStreamCreate...() functions and FSEventStreamCallback(). They are monotonically increasing per system, even across reboots and drives coming and going. They bear no relation to any particular clock or timebase.

