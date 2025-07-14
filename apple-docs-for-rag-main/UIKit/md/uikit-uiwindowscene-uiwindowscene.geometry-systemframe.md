

- UIKit
- UIWindowScene
- UIWindowScene.Geometry
-  systemFrame 

Instance Property

# systemFrame

The current frame of the scene, in system coordinates.

Mac Catalyst 16.0+

``` source
var systemFrame: CGRect { get }
```

## Discussion

This property represents the current frame of the scene in the system coordinate space, where an origin of `(0, 0)` corresponds to the top-left corner of the main display.

## See Also

### Accessing scene geometry

var interfaceOrientation: UIInterfaceOrientation

The current interface orientation for the scene.

