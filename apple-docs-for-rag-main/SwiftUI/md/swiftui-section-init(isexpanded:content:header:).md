

- SwiftUI
- Section
-  init(isExpanded:content:header:) 

Initializer

# init(isExpanded:content:header:)

Creates a section with a header, the provided section content, and a binding representing the section’s expansion state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    isExpanded: Binding,
    @ViewBuilder content: () -> Content,
    @ViewBuilder header: () -> Parent
)
```

Available when `Parent` conforms to `View`, `Content` conforms to `View`, and `Footer` is `EmptyView`.

Show all declarations

## Parameters 

`isExpanded`  

A binding to a Boolean value that determines the section’s expansion state (expanded or collapsed).

`content`  

The section’s content.

`header`  

A view to use as the section’s header.

## See Also

### Controlling collapsibility

init(_:isExpanded:content:)

Creates a section with the provided section content.

