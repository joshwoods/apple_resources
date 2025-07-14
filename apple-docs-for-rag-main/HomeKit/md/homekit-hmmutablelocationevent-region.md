

- HomeKit
- HMMutableLocationEvent
-  region 

Instance Property

# region

The region on which events are triggered.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+watchOS 4.0+

``` source
var region: CLRegion? { get set }
```

## Discussion

Use this property to set the region on which the location event is triggered. The region object must have at least one of notifyOnEntry or notifyOnExit set to true.

This property is `nil` when an application is not authorized for location services.

