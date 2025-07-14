

- SwiftUI
- Scene
-  windowToolbarLabelStyle(\_:) 

Instance Method

# windowToolbarLabelStyle(\_:)

Sets the label style of items in a toolbar and enables user customization.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func windowToolbarLabelStyle(_ toolbarLabelStyle: Binding) -> some Scene
```

## Parameters 

`toolbarLabelStyle`  

The label style to apply.

## Discussion

Use this modifier to bind a ToolbarLabelStyle to AppStorage. The toolbar will default to the label style specified but will also be user configurable.

```
    @main
    struct MyApp: App {
        @AppStorage("ToolbarLabelStyle")
        private var labelStyle: ToolbarLabelStyle = .iconOnly

        var body: some Scene {
            WindowGroup {
                ContentView()
                    .toolbar(id: "browserToolbar") {
                        ...
                    }
            }
            .windowToolbarLabelStyle($labelStyle)
        }
    }
```

## See Also

### Styling the associated toolbar

func windowToolbarStyle&lt;S>(S) -> some Scene

Sets the style for the toolbar defined within this scene.

func windowToolbarLabelStyle(fixed: ToolbarLabelStyle) -> some Scene

Sets the label style of items in a toolbar.

protocol WindowToolbarStyle

A specification for the appearance and behavior of a window’s toolbar.

