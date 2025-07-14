

- UIKit
- UIWindowScene
- UIWindowScene.GeometryPreferences
- UIWindowScene.GeometryPreferences.Mac
-  systemFrame 

Instance Property

# systemFrame

The preferred frame of the scene, in system coordinates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS

``` source
var systemFrame: CGRect? { get set }
```

## Discussion

This property represents the preferred frame of the scene in the system coordinate space, where an origin of `(0, 0)` corresponds to the top-left corner of the main display. The default value is CGRectNull, which indicates no preferred frame.

