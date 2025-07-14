

- SwiftUI
- NavigationLink
-  init(destination:label:) 

Initializer

# init(destination:label:)

Creates a navigation link that presents the destination view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    @ViewBuilder destination: () -> Destination,
    @ViewBuilder label: () -> Label
)
```

Show all declarations

## Parameters 

`destination`  

A view for the navigation link to present.

`label`  

A view builder to produce a label describing the `destination` to present.

## See Also

### Presenting a destination view

init(_:destination:)

Creates a navigation link that presents a destination view, with a text label that the link generates from a localized string key.

