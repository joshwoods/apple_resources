

- Core Location
- CLLocationUpdate
-  liveUpdates(\_:) 

Type Method

# liveUpdates(\_:)

Tells Core Location to start delivering the location updates it produces for the configuration you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func liveUpdates(_ configuration: CLLocationUpdate.LiveConfiguration = .default) -> CLLocationUpdate.Updates
```

## Parameters 

`configuration`  

A configuration that describes the updates for the framework to deliver.

## Return Value

CLLocationUpdate.Updates that meet the criteria you specify.

## See Also

### Receiving location updates

enum LiveConfiguration

Values for indicating the kind of updates the framework delivers.

struct Updates

A structure that represents an asynchronous sequence of location updates.

