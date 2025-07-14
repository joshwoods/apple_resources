

- SwiftUI
- ScrollPosition
-  init(id:anchor:) 

Initializer

# init(id:anchor:)

Creates a new scroll position to a view with a provided identity value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    id: some Hashable & Sendable,
    anchor: UnitPoint? = nil
)
```

## Discussion

The type of the ID indicates the type of ID of views within a scroll target layout the scroll view should look for.

