

- SwiftUI
- TabContent
-  draggable(\_:) 

Instance Method

# draggable(\_:)

Activates this tab as the source of a drag and drop operation. This tab can only be dragged when in the sidebar.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.1+

``` source
@MainActor @preconcurrency
func draggable(_ payload: @autoclosure @escaping () -> T) -> some TabContent where T : Transferable
```

## Parameters 

`payload`  

A closure that returns a single instance or a value conforming to Transferable that represents the draggable data from this tab.

## Discussion

Applying the `draggable(_:)` modifier adds the appropriate gestures for drag and drop to this tab. When a drag operation begins, a rendering of the tab is generated and used as the preview image.

The following example allows the ‘Family’ tab to be dragged and dropped.

```
TabView {
    Tab("Family", systemImage: "list.bullet") {
        MyFamilyView()
    }
    .draggable(AppSections.family)
}
```

