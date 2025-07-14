

- SwiftUI
- NavigationLink
-  init(\_:destination:) 

Initializer

# init(\_:destination:)

Creates a navigation link that presents a destination view, with a text label that the link generates from a localized string key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder destination: () -> Destination
)
```

Available when `Label` is `Text` and `Destination` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

A localized string key for creating a text label.

`destination`  

A view for the navigation link to present.

## See Also

### Presenting a destination view

init(destination:label:)

Creates a navigation link that presents the destination view.

