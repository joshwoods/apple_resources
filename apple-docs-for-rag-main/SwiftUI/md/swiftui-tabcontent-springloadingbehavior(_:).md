

- SwiftUI
- TabContent
-  springLoadingBehavior(\_:) 

Instance Method

# springLoadingBehavior(\_:)

Sets the spring loading behavior for the tab.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func springLoadingBehavior(_ behavior: SpringLoadingBehavior) -> some TabContent
```

## Parameters 

`behavior`  

Whether spring loading is enabled or not. If unspecified, the default behavior is `.automatic.`

## Discussion

Spring loading refers to a view being activated during a drag and drop interaction. On iOS this can occur when pausing briefly on top of a view with dragged content. On macOS this can occur with similar brief pauses or on pressure-sensitive systems by “force clicking” during the drag. This has no effect on tvOS or watchOS.

This is commonly used with views that have a navigation or presentation effect, allowing the destination to be revealed without pausing the drag interaction. For example, a button that reveals a list of folders that a dragged item can be dropped onto.

Unlike `disabled(_:)`, this modifier overrides the value set by an ancestor view rather than being unioned with it. For example, the tab below would allow spring loading:

```
TabView {
    Tab("Favorites", systemImage: "star") {
        MyFavoritesView()
    }
    .springLoadingBehavior(.enabled)

    ...
}
.springLoadingBehavior(.disabled)
```

