

- SwiftUI
- ScrollPosition
-  init(idType:edge:) 

Initializer

# init(idType:edge:)

Creates a new scroll position to be scrolled to the provided edge.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    idType: (some Hashable & Sendable).Type = Never.self,
    edge: Edge
)
```

## Discussion

You can provide a type to indicate the type of ID the scroll view should look for views with an ID of that type within its scroll target layout.

