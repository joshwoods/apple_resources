

- SwiftUI
- Scene
-  menuBarExtraStyle(\_:) 

Instance Method

# menuBarExtraStyle(\_:)

Sets the style for menu bar extra created by this scene.

macOS 13.0+

``` source
nonisolated
func menuBarExtraStyle(_ style: S) -> some Scene where S : MenuBarExtraStyle
```

## See Also

### Creating a menu bar extra

struct MenuBarExtra

A scene that renders itself as a persistent control in the system menu bar.

protocol MenuBarExtraStyle

A specification for the appearance and behavior of a menu bar extra scene.

