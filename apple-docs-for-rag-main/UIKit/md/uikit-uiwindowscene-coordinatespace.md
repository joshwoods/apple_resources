

- UIKit
- UIWindowScene
-  coordinateSpace 

Instance Property

# coordinateSpace

The coordinate space occupied by the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var coordinateSpace: any UICoordinateSpace { get }
```

## Discussion

Use the provided coordinate space to get the bounds of the scene’s bounds rectangle and to convert points and rectangles to and from other coordinate spaces. For example, use coordinateSpace to convert a point in the scene to the screen coordinate space.

## See Also

### Getting the interface attributes

var traitCollection: UITraitCollection

The traits that describe the current environment of the scene.

var interfaceOrientation: UIInterfaceOrientation

The orientation to use when displaying content in your windows.

var sizeRestrictions: UISceneSizeRestrictions?

The minimum and maximum size of the app’s windows.

class UISceneSizeRestrictions

An object that specifies the minimum and maximum sizes for resizable windows.

