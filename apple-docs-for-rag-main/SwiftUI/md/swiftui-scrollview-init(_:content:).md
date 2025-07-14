

- SwiftUI
- ScrollView
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a new instance that’s scrollable in the direction of the given axis and can show indicators while scrolling.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(
    _ axes: Axis.Set = .vertical,
    @ViewBuilder content: () -> Content
)
```

Available when `Content` conforms to `View`.

## Parameters 

`axes`  

The scroll view’s scrollable axis. The default axis is the vertical axis.

`content`  

The view builder that creates the scrollable view.

## See Also

### Creating a scroll view

init(Axis.Set, showsIndicators: Bool, content: () -> Content)

Creates a new instance that’s scrollable in the direction of the given axis and can show indicators while scrolling.

Deprecated

