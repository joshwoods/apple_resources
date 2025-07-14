

- SwiftUI
- CommandGroup
-  init(replacing:addition:) 

Initializer

# init(replacing:addition:)

A value describing the complete replacement of the contents of the indicated group with the given views.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    replacing group: CommandGroupPlacement,
    @ViewBuilder addition: () -> Content
)
```

## See Also

### Creating a command group

init(after: CommandGroupPlacement, addition: () -> Content)

A value describing the addition of the given views to the end of the indicated group.

init(before: CommandGroupPlacement, addition: () -> Content)

A value describing the addition of the given views to the beginning of the indicated group.

