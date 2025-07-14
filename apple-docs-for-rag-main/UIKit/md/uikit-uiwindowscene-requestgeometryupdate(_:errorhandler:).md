

- UIKit
- UIWindowScene
-  requestGeometryUpdate(\_:errorHandler:) 

Instance Method

# requestGeometryUpdate(\_:errorHandler:)

Requests an update to the window scene’s geometry using the specified geometry preferences object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
func requestGeometryUpdate(
    _ geometryPreferences: UIWindowScene.GeometryPreferences,
    errorHandler: ((any Error) -> Void)? = nil
)
```

## Parameters 

`geometryPreferences`  

The geometry information to use for the request.

`errorHandler`  

An optional closure to call when an error occurs. The system may call the error handler asynchronously.

## Discussion

Use this method to explicitly request geometry changes to the window scene. The following code shows an example of requesting the window scene to rotate to a landscape orientation in iOS.

```
// In a view controller, get the window scene.
guard let windowScene = view.window?.windowScene else { return }

// Request the window scene to rotate to any landscape orientation.
windowScene.requestGeometryUpdate(.iOS(interfaceOrientations: .landscape)) { error in
    // Handle denial of request.
}
```

## See Also

### Working with window geometry

var effectiveGeometry: UIWindowScene.Geometry

The current values for the window scene’s geometry in system space.

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

