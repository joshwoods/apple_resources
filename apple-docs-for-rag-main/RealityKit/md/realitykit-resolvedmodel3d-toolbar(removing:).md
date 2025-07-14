

- RealityKit
- ResolvedModel3D
-  toolbar(removing:) 

Instance Method

# toolbar(removing:)

Remove a toolbar item present by default

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
nonisolated
func toolbar(removing defaultItemKind: ToolbarDefaultItemKind?) -> some View
```

## Parameters 

`defaultItemKind`  

The kind of default item to remove

## Discussion

Use this modifier to remove toolbar items other `View`s add by default. For example, to remove the sidebar toggle toolbar item provided by `NavigationSplitView`:

```
NavigationSplitView {
    SidebarView()
        .toolbar(removing: .sidebarToggle)
} detail: {
    DetailView()
}
```

