

- SwiftUI
- Scene
-  windowToolbarStyle(\_:) 

Instance Method

# windowToolbarStyle(\_:)

Sets the style for the toolbar defined within this scene.

macOS 11.0+

``` source
nonisolated
func windowToolbarStyle(_ style: S) -> some Scene where S : WindowToolbarStyle
```

## See Also

### Styling a toolbar

func toolbarBackground(_:for:)

Specifies the preferred shape style of the background of a bar managed by SwiftUI.

func toolbarColorScheme(ColorScheme?, for: ToolbarPlacement...) -> some View

Specifies the preferred color scheme of a bar managed by SwiftUI.

func toolbarForegroundStyle&lt;S>(S, for: ToolbarPlacement...) -> some View

Specifies the preferred foreground style of bars managed by SwiftUI.

protocol WindowToolbarStyle

A specification for the appearance and behavior of a window’s toolbar.

var toolbarLabelStyle: ToolbarLabelStyle?

The label style to apply to controls within a toolbar.

struct ToolbarLabelStyle

The label style of a toolbar.

