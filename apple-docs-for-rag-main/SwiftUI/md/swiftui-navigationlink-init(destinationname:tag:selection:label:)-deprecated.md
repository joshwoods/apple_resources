

- SwiftUI
- NavigationLink
-  init(destinationName:tag:selection:label:) Deprecated

Initializer

# init(destinationName:tag:selection:label:)

Creates a navigation link that presents a view from a WatchKit storyboard when a bound selection variable matches a value you provide.

watchOS 6.0–11.4Deprecated

``` source
nonisolated
init(
    destinationName: String,
    tag: V,
    selection: Binding,
    @ViewBuilder label: () -> Label
) where V : Hashable
```

Available when `Label` conforms to `View` and `Destination` is `_WKStoryboardContent`.

Deprecated

Use init(value:label:) inside a List within a NavigationStack or NavigationSplitView. For more information, see Migrating to new navigation types.

## Parameters 

`destinationName`  

The storyboard name of a view for the navigation link to present.

`tag`  

The value of `selection` that causes the link to present `destination`.

`selection`  

A bound variable that causes the link to present `destination` when `selection` becomes equal to `tag`.

`label`  

A view builder to produce a label describing the `destination` to present.

## See Also

### Creating links for WatchKit

init(destinationName: String, isActive: Binding&lt;Bool>, label: () -> Label)

Creates a navigation link that presents a view from a WatchKit storyboard when active.

Deprecated

init(destinationName: String, label: () -> Label)

Creates a navigation link that presents a view from a WatchKit storyboard.

Deprecated

