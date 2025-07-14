

- SwiftUI
- NavigationLink
-  init(\_:destination:tag:selection:) Deprecated

Initializer

# init(\_:destination:tag:selection:)

Creates a navigation link that presents a destination view when a bound selection variable matches a value you provide, using a text label that the link generates from a title string.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.0–16.0DeprecatedmacOS 10.15–13.0DeprecatedtvOS 13.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 6.0–9.0Deprecated

``` source
nonisolated
init(
    _ title: S,
    destination: Destination,
    tag: V,
    selection: Binding
) where S : StringProtocol, V : Hashable
```

Available when `Label` is `Text` and `Destination` conforms to `View`.

Deprecated

Use init(_:value:) inside a List within a NavigationStack or NavigationSplitView. For more information, see Migrating to new navigation types.

Show all declarations

## Parameters 

`title`  

A string for creating a text label.

`destination`  

A view for the navigation link to present.

`tag`  

The value of `selection` that causes the link to present `destination`.

`selection`  

A bound variable that causes the link to present `destination` when `selection` becomes equal to `tag`.

## See Also

### Creating links with view arguments

init(_:destination:isActive:)

Creates a navigation link that presents a destination view when active, with a text label that the link generates from a localized string key.

Deprecated

init(destination: Destination, isActive: Binding&lt;Bool>, label: () -> Label)

Creates a navigation link that presents the destination view when active.

Deprecated

init&lt;V>(destination: Destination, tag: V, selection: Binding&lt;V?>, label: () -> Label)

Creates a navigation link that presents the destination view when a bound selection variable equals a given tag value.

Deprecated

