

- SwiftUI
- AnyLayout
-  init(\_:) 

Initializer

# init(\_:)

Creates a type-erased value that wraps the specified layout.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(_ layout: L) where L : Layout
```

## Discussion

You can switch between type-erased layouts without losing the state of the subviews.

