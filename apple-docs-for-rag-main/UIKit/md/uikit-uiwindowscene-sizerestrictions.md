

- UIKit
- UIWindowScene
-  sizeRestrictions 

Instance Property

# sizeRestrictions

The minimum and maximum size of the app’s windows.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var sizeRestrictions: UISceneSizeRestrictions? { get }
```

## Discussion

When the value of this property is not `nil`, use it to change the default minimum and maximum window sizes for your app. If the value of this property is `nil,` the system doesn’t allow you to set window size restrictions.

## See Also

### Getting the interface attributes

var traitCollection: UITraitCollection

The traits that describe the current environment of the scene.

var coordinateSpace: any UICoordinateSpace

The coordinate space occupied by the scene.

var interfaceOrientation: UIInterfaceOrientation

The orientation to use when displaying content in your windows.

class UISceneSizeRestrictions

An object that specifies the minimum and maximum sizes for resizable windows.

