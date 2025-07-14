

- SwiftUI
- AsymmetricTransition
-  init(insertion:removal:) 

Initializer

# init(insertion:removal:)

Creates a composite `Transition` that uses a different transition for insertion versus removal.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    insertion: Insertion,
    removal: Removal
)
```

