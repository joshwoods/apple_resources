

- UIKit
- UICoordinateSpace
-  bounds 

Instance Property

# bounds

The bounds rectangle describing the item’s location and size in its own coordinate system.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var bounds: CGRect { get }
```

**Required**

## Discussion

The rectangle in this property always matches the app’s interface orientation. For apps that support all interface orientations, the value in this property can change when the user rotates the device between portrait and landscape modes.

