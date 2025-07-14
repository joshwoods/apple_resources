

- UIKit
- UIWindowScene
-  interfaceOrientation 

Instance Property

# interfaceOrientation

The orientation to use when displaying content in your windows.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var interfaceOrientation: UIInterfaceOrientation { get }
```

## Discussion

The interface orientation normally corresponds to the device orientation, but it might also be different. For example, the interface orientation does not always match the device orientation when the user enables rotation lock for the device.

## See Also

### Getting the interface attributes

var traitCollection: UITraitCollection

The traits that describe the current environment of the scene.

var coordinateSpace: any UICoordinateSpace

The coordinate space occupied by the scene.

var sizeRestrictions: UISceneSizeRestrictions?

The minimum and maximum size of the app’s windows.

class UISceneSizeRestrictions

An object that specifies the minimum and maximum sizes for resizable windows.

