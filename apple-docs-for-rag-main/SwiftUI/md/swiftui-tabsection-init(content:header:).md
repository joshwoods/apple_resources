

- SwiftUI
- TabSection
-  init(content:header:) 

Initializer

# init(content:header:)

Creates a section with a header and the provided section content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    @TabContentBuilder content: () -> Content,
    @ViewBuilder header: () -> Header
) where Header : View, Footer == EmptyView
```

Available when `Content` conforms to `TabContent` and `SelectionValue` conforms to `Hashable`.

Show all declarations

## Parameters 

`content`  

The section’s content.

`header`  

A view to use as the section’s header.

## See Also

### Creating a tab section

init(content:)

Creates a section with the provided section content.

init(_:content:)

Creates a section with the provided content.

