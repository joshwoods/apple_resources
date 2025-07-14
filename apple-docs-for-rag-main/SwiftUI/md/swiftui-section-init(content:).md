

- SwiftUI
- Section
-  init(content:) 

Initializer

# init(content:)

Creates a section with the provided section content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(@ViewBuilder content: () -> Content)
```

Available when `Parent` is `EmptyView`, `Content` conforms to `View`, and `Footer` is `EmptyView`.

Show all declarations

## Parameters 

`content`  

The section’s content.

## See Also

### Creating a section

init(_:content:)

Creates a section with the provided section content.

