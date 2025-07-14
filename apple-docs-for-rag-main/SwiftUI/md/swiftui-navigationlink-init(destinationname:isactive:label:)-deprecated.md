

- SwiftUI
- NavigationLink
-  init(destinationName:isActive:label:) Deprecated

Initializer

# init(destinationName:isActive:label:)

Creates a navigation link that presents a view from a WatchKit storyboard when active.

watchOS 6.0–11.4Deprecated

``` source
nonisolated
init(
    destinationName: String,
    isActive: Binding,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View` and `Destination` is `_WKStoryboardContent`.

Deprecated

Use init(value:label:) instead. For more information, see Migrating to new navigation types.

## Parameters 

`destinationName`  

The storyboard name of a view for the navigation link to present.

`isActive`  

A binding to a Boolean value that indicates whether `destination` is currently presented.

`label`  

A view builder to produce a label describing the `destination` to present.

## See Also

### Creating links for WatchKit

init&lt;V>(destinationName: String, tag: V, selection: Binding&lt;V?>, label: () -> Label)

Creates a navigation link that presents a view from a WatchKit storyboard when a bound selection variable matches a value you provide.

Deprecated

init(destinationName: String, label: () -> Label)

Creates a navigation link that presents a view from a WatchKit storyboard.

Deprecated

