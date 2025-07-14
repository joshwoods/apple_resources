

- UIKit
- UIWindowScene
- UIWindowScene.GeometryPreferences
-  UIWindowScene.GeometryPreferences.iOS 

Class

# UIWindowScene.GeometryPreferences.iOS

An object that represents the geometry preferences for a window scene in an iOS app.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class iOS
```

## Overview

Use this class to express iOS-specific geometry preferences when you call requestGeometryUpdate(_:errorHandler:).

## Topics

### Creating a geometry preferences object

convenience init(interfaceOrientations: UIInterfaceOrientationMask)

Initializes a new window scene geometry preferences object with the specified interface orientations.

init()

Initializes a new window scene geometry preferences object.

### Requesting preferred interface orientations

var interfaceOrientations: UIInterfaceOrientationMask?

The preferred interface orientations for the scene.

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

### Related Documentation

var effectiveGeometry: UIWindowScene.Geometry

The current values for the window scene’s geometry in system space.

func requestGeometryUpdate(UIWindowScene.GeometryPreferences, errorHandler: ((any Error) -> Void)?)

Requests an update to the window scene’s geometry using the specified geometry preferences object.

### Working with window geometry

var effectiveGeometry: UIWindowScene.Geometry

The current values for the window scene’s geometry in system space.

func requestGeometryUpdate(UIWindowScene.GeometryPreferences, errorHandler: ((any Error) -> Void)?)

Requests an update to the window scene’s geometry using the specified geometry preferences object.

class Geometry

An object that provides geometry information about the window scene.

class GeometryPreferences

An abstract superclass for representing window scene geometry preferences.

class Mac

An object that represents the geometry preferences for a window scene in an app built with Mac Catalyst.

class Vision

let UIProposedSceneSizeNoPreference: CGFloat

