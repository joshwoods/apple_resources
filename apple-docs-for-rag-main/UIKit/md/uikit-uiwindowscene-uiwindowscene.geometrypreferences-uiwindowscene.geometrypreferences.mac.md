

- UIKit
- UIWindowScene
- UIWindowScene.GeometryPreferences
-  UIWindowScene.GeometryPreferences.Mac 

Class

# UIWindowScene.GeometryPreferences.Mac

An object that represents the geometry preferences for a window scene in an app built with Mac Catalyst.

iOSiPadOSMac Catalyst 16.0+tvOSvisionOS

``` source
class Mac
```

## Overview

Use this class to express macOS-specific geometry preferences when you call requestGeometryUpdate(_:errorHandler:).

## Topics

### Creating a geometry preferences object

convenience init(systemFrame: CGRect)

Initializes a new window scene geometry preferences object with the specified window frame.

init()

Initializes a new window scene geometry preferences object.

### Accessing geometry information

var systemFrame: CGRect?

The preferred frame of the scene, in system coordinates.

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

class iOS

An object that represents the geometry preferences for a window scene in an iOS app.

class Vision

let UIProposedSceneSizeNoPreference: CGFloat

