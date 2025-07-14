

- Game Controller
- GCDeviceHaptics
-  createEngine(withLocality:) 

Instance Method

# createEngine(withLocality:)

Creates a haptics engine with the specified locality.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func createEngine(withLocality locality: GCHapticsLocality) -> CHHapticEngine?
```

## Parameters 

`locality`  

The location of the haptics on the controller.

## Return Value

A new haptics engine with the specified locality.

## Discussion

If you create an engine using the default location, users have the expected haptic experience. For example, the engine uses the handle accuators. If you want to create different experiences, such as using the left handle actuator as a woofer and the right actuator as a tweeter, create one or more engines with different localities.

## See Also

### Creating a haptics engine

let GCHapticDurationInfinite: Float

An infinite duration for a haptics event.

