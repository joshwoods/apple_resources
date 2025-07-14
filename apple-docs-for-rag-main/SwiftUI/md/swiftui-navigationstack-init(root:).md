

- SwiftUI
- NavigationStack
-  init(root:) 

Initializer

# init(root:)

Creates a navigation stack that manages its own navigation state.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
init(@ViewBuilder root: () -> Root) where Data == NavigationPath
```

## Parameters 

`root`  

The view to display when the stack is empty.

