

- UIKit
- UITraitCollection
-  forceTouchCapability 

Instance Property

# forceTouchCapability

The force touch capability value of the trait collection.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var forceTouchCapability: UIForceTouchCapability { get }
```

## Mentioned in 

Checking the availability of 3D Touch

## Discussion

3D Touch is available only on certain devices. On those devices, availability is determined by the user’s associated accessibility setting in the Settings app. Check this property’s value on app launch, and in your implementation of the traitCollectionDidChange(_:) method.

If this property does not contain a value, the meaning is equivalent to the value UIForceTouchCapability.unknown.

## See Also

### Retrieving the force touch capability traits

enum UIForceTouchCapability

Keys that indicate the availability of 3D Touch on a device.

