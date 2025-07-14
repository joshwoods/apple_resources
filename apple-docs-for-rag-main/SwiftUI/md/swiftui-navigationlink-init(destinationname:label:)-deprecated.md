

- SwiftUI
- NavigationLink
-  init(destinationName:label:) Deprecated

Initializer

# init(destinationName:label:)

Creates a navigation link that presents a view from a WatchKit storyboard.

watchOS 6.0–11.4Deprecated

``` source
nonisolated
init(
    destinationName: String,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View` and `Destination` is `_WKStoryboardContent`.

Deprecated

Use init(destination:label:) instead.

## Parameters 

`destinationName`  

The storyboard name of a view for the navigation link to present.

`label`  

A view builder to produce a label describing the `destination` to present.

## See Also

### Creating links for WatchKit

init(destinationName: String, isActive: Binding&lt;Bool>, label: () -> Label)

Creates a navigation link that presents a view from a WatchKit storyboard when active.

Deprecated

init&lt;V>(destinationName: String, tag: V, selection: Binding&lt;V?>, label: () -> Label)

Creates a navigation link that presents a view from a WatchKit storyboard when a bound selection variable matches a value you provide.

Deprecated

