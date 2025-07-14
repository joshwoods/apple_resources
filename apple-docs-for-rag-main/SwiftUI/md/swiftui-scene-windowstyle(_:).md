

- SwiftUI
- Scene
-  windowStyle(\_:) 

Instance Method

# windowStyle(\_:)

Sets the style for windows created by this scene.

macOS 11.0+visionOS 1.0+

``` source
nonisolated
func windowStyle(_ style: S) -> some Scene where S : WindowStyle
```

## See Also

### Creating windows

struct WindowGroup

A scene that presents a group of identically structured windows.

struct Window

A scene that presents its content in a single, unique window.

struct UtilityWindow

A specialized window scene that provides secondary utility to the content of the main scenes of an application.

protocol WindowStyle

A specification for the appearance and interaction of a window.

