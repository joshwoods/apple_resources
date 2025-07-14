

- UIKit
- UIWindowScene
-  traitCollection 

Instance Property

# traitCollection

The traits that describe the current environment of the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var traitCollection: UITraitCollection { get }
```

## Discussion

Use this property to get additional information about the current scene, such as the size class and scale factor. For more information about the available traits, see UITraitCollection.

## See Also

### Getting the interface attributes

var coordinateSpace: any UICoordinateSpace

The coordinate space occupied by the scene.

var interfaceOrientation: UIInterfaceOrientation

The orientation to use when displaying content in your windows.

var sizeRestrictions: UISceneSizeRestrictions?

The minimum and maximum size of the app’s windows.

class UISceneSizeRestrictions

An object that specifies the minimum and maximum sizes for resizable windows.

