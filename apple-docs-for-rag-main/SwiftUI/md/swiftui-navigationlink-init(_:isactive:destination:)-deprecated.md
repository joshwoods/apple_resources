

- SwiftUI
- NavigationLink
-  init(\_:isActive:destination:) Deprecated

Initializer

# init(\_:isActive:destination:)

Creates a navigation link that presents a destination view when active, with a text label that the link generates from a localized string key.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.0–16.0DeprecatedmacOS 10.15–13.0DeprecatedtvOS 13.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 6.0–9.0Deprecated

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    isActive: Binding,
    @ViewBuilder destination: () -> Destination
)
```

Available when `Label` is `Text` and `Destination` conforms to `View`.

Deprecated

Use init(_:value:) inside a NavigationStack or NavigationSplitView. For more information, see Migrating to new navigation types.

Show all declarations

## Parameters 

`titleKey`  

A localized string key for creating a text label.

`isActive`  

A binding to a Boolean value that indicates whether `destination` is currently presented.

`destination`  

A view for the navigation link to present.

## See Also

### Creating links with view builders

init(isActive: Binding&lt;Bool>, destination: () -> Destination, label: () -> Label)

Creates a navigation link that presents the destination view when active.

Deprecated

init(_:tag:selection:destination:)

Creates a navigation link that presents a destination view when a bound selection variable matches a value you provide, using a text label that the link generates from a title string.

Deprecated

init&lt;V>(tag: V, selection: Binding&lt;V?>, destination: () -> Destination, label: () -> Label)

Creates a navigation link that presents the destination view when a bound selection variable equals a given tag value.

Deprecated

