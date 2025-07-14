

- UIKit
- UIWindowScene
- UIWindowScene.GeometryPreferences
-  UIWindowScene.GeometryPreferences.Vision 

Class

# UIWindowScene.GeometryPreferences.Vision

visionOS 1.0+

``` source
class Vision
```

## Topics

### Initializers

init()

convenience init(size: CGSize?, minimumSize: CGSize?, maximumSize: CGSize?, resizingRestrictions: UIWindowScene.ResizingRestrictions?)

### Instance Properties

var maximumSize: CGSize?

var minimumSize: CGSize?

var resizingRestrictions: UIWindowScene.ResizingRestrictions?

var size: CGSize?

## Relationships

### Inherits From

- UIWindowScene.GeometryPreferences

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Working with window geometry

var effectiveGeometry: UIWindowScene.Geometry

The current values for the window scene’s geometry in system space.

func requestGeometryUpdate(UIWindowScene.GeometryPreferences, errorHandler: ((any Error) -> Void)?)

Requests an update to the window scene’s geometry using the specified geometry preferences object.

class Geometry

An object that provides geometry information about the window scene.

class GeometryPreferences

An abstract superclass for representing window scene geometry preferences.

class iOS

An object that represents the geometry preferences for a window scene in an iOS app.

class Mac

An object that represents the geometry preferences for a window scene in an app built with Mac Catalyst.

let UIProposedSceneSizeNoPreference: CGFloat

