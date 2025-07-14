

- SwiftUI
- Section
-  init(content:footer:) 

Initializer

# init(content:footer:)

Creates a section with a footer and the provided section content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    @ViewBuilder content: () -> Content,
    @ViewBuilder footer: () -> Footer
)
```

Available when `Parent` is `EmptyView`, `Content` conforms to `View`, and `Footer` conforms to `View`.

## Parameters 

`content`  

The section’s content.

`footer`  

A view to use as the section’s footer.

## See Also

### Adding headers and footers

init(content:header:)

Creates a section with a header and the provided section content.

init(content: () -> Content, header: () -> Parent, footer: () -> Footer)

Creates a section with a header, footer, and the provided section content.

