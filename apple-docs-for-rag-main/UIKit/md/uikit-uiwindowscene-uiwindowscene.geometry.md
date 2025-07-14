

- UIKit
- UIWindowScene
-  UIWindowScene.Geometry 

Class

# UIWindowScene.Geometry

An object that provides geometry information about the window scene.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
class Geometry
```

## Topics

### Accessing scene geometry

var systemFrame: CGRect

The current frame of the scene, in system coordinates.

var interfaceOrientation: UIInterfaceOrientation

The current interface orientation for the scene.

### Instance Properties

var maximumSize: CGSize

var minimumSize: CGSize

var resizingRestrictions: UIWindowSceneResizingRestrictions

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Working with window geometry

var effectiveGeometry: UIWindowScene.Geometry

The current values for the window scene’s geometry in system space.

func requestGeometryUpdate(UIWindowScene.GeometryPreferences, errorHandler: ((any Error) -> Void)?)

Requests an update to the window scene’s geometry using the specified geometry preferences object.

class GeometryPreferences

An abstract superclass for representing window scene geometry preferences.

class iOS

An object that represents the geometry preferences for a window scene in an iOS app.

class Mac

An object that represents the geometry preferences for a window scene in an app built with Mac Catalyst.

class Vision

let UIProposedSceneSizeNoPreference: CGFloat

