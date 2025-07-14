

- SwiftUI
- ScrollViewReader
-  init(content:) 

Initializer

# init(content:)

Creates an instance that can perform programmatic scrolling of its child scroll views.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(@ViewBuilder content: @escaping (ScrollViewProxy) -> Content)
```

## Parameters 

`content`  

The reader’s content, containing one or more scroll views. This view builder receives a ScrollViewProxy instance that you use to perform scrolling.

