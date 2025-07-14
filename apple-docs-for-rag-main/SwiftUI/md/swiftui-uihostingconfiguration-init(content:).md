

- SwiftUI
- UIHostingConfiguration
-  init(content:) 

Initializer

# init(content:)

Creates a hosting configuration with the given contents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
init(@ViewBuilder content: () -> Content)
```

Available when `Content` conforms to `View` and `Background` is `EmptyView`.

## Parameters 

`content`  

The contents of the SwiftUI hierarchy to be shown inside the cell.

