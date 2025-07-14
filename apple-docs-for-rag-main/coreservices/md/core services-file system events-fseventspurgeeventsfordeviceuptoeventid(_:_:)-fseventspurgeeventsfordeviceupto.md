

- Core Services
- File System Events
-  FSEventsPurgeEventsForDeviceUpToEventId(\_:\_:) 

Function

# FSEventsPurgeEventsForDeviceUpToEventId(\_:\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func FSEventsPurgeEventsForDeviceUpToEventId(
    _ dev: dev_t,
    _ eventId: FSEventStreamEventId
) -> Bool
```

## Parameters 

`dev`  

The dev_t of the device.

`eventId`  

The event ID.

## Return Value

True if it succeeds, otherwise False if it fails.

## Discussion

Purges old events from the persistent per-volume database maintained by the service. Can only be called by the root user.

