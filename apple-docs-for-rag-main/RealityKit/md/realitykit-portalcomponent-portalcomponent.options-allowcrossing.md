

- RealityKit
- PortalComponent
- PortalComponent.Options
-  allowCrossing 

Type Property

# allowCrossing

An option that enables the crossing feature.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static let allowCrossing: PortalComponent.Options
```

## Discussion

Objects within the portal world with a PortalCrossingComponent can cross the portal when the `allowCrossing` option is in an enabled state. Crossing behavior is based on the user-defined geometry for crossingMode.

