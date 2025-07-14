

- RealityKit
- ObjectCaptureView
-  toolbarTitleDisplayMode(\_:) 

Instance Method

# toolbarTitleDisplayMode(\_:)

Configures the toolbar title display mode for this view.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
func toolbarTitleDisplayMode(_ mode: ToolbarTitleDisplayMode) -> some View
```

## Discussion

Use this modifier to override the default toolbar title display mode.

```
NavigationStack {
    ContentView()
        .toolbarTitleDisplayMode(.inlineLarge)
}
```

See `ToolbarTitleDisplayMode` for more information on the different kinds of display modes. This modifier has no effect on macOS.

