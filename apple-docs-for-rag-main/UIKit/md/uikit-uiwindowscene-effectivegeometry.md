

- UIKit
- UIWindowScene
-  effectiveGeometry 

Instance Property

# effectiveGeometry

The current values for the window scene’s geometry in system space.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var effectiveGeometry: UIWindowScene.Geometry { get }
```

## Discussion

This property is key-value observing (KVO) compliant. Observing effectiveGeometry is the recommended way to receive notifications of changes to the window scene’s geometry. These changes can occur because of user interaction or as a result of the system resolving a geometry request.

## See Also

### Working with window geometry

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

class Vision

let UIProposedSceneSizeNoPreference: CGFloat

