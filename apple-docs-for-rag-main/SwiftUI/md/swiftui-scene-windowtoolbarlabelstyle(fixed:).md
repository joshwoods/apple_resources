

- SwiftUI
- Scene
-  windowToolbarLabelStyle(fixed:) 

Instance Method

# windowToolbarLabelStyle(fixed:)

Sets the label style of items in a toolbar.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func windowToolbarLabelStyle(fixed: ToolbarLabelStyle) -> some Scene
```

## Discussion

Use this modifier to set a static ToolbarLabelStyle the toolbar should use. The style will not be configurable by the user.

```
    @main
    struct MyApp: App {
        var body: some Scene {
            WindowGroup {
                ContentView()
                    .toolbar(id: "browserToolbar") {
                        ...
                    }
            }
            .windowToolbarLabelStyle(fixed: .iconOnly)
        }
    }
```

## See Also

### Styling the associated toolbar

func windowToolbarStyle&lt;S>(S) -> some Scene

Sets the style for the toolbar defined within this scene.

func windowToolbarLabelStyle(Binding&lt;ToolbarLabelStyle>) -> some Scene

Sets the label style of items in a toolbar and enables user customization.

protocol WindowToolbarStyle

A specification for the appearance and behavior of a window’s toolbar.

