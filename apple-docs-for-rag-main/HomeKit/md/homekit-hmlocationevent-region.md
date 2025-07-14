

- HomeKit
- HMLocationEvent
-  region 

Instance Property

# region

The region on which events are triggered.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+watchOS 2.0+

``` source
var region: CLRegion? { get }
```

## Discussion

The event is triggered based on the values of the notifyOnEntry and notifyOnExit properties.

This property is `nil` when an application is not authorized for location services.

