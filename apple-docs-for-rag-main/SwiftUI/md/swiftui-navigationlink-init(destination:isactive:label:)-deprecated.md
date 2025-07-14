

- SwiftUI
- NavigationLink
-  init(destination:isActive:label:) Deprecated

Initializer

# init(destination:isActive:label:)

Creates a navigation link that presents the destination view when active.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.0–16.0DeprecatedmacOS 10.15–13.0DeprecatedtvOS 13.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 6.0–9.0Deprecated

``` source
init(
    destination: Destination,
    isActive: Binding,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View` and `Destination` conforms to `View`.

Deprecated

Use init(value:label:) instead. For more information, see Migrating to new navigation types.

## Parameters 

`destination`  

A view for the navigation link to present.

`isActive`  

A binding to a Boolean value that indicates whether `destination` is currently presented.

`label`  

A view builder to produce a label describing the `destination` to present.

## See Also

### Creating links with view arguments

init(_:destination:isActive:)

Creates a navigation link that presents a destination view when active, with a text label that the link generates from a localized string key.

Deprecated

init(_:destination:tag:selection:)

Creates a navigation link that presents a destination view when a bound selection variable matches a value you provide, using a text label that the link generates from a title string.

Deprecated

init&lt;V>(destination: Destination, tag: V, selection: Binding&lt;V?>, label: () -> Label)

Creates a navigation link that presents the destination view when a bound selection variable equals a given tag value.

Deprecated

