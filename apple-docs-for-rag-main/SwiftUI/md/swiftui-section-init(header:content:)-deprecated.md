

- SwiftUI
- Section
-  init(header:content:) Deprecated

Initializer

# init(header:content:)

Creates a section with a header and the provided section content.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
init(
    header: Parent,
    @ViewBuilder content: () -> Content
)
```

Available when `Parent` conforms to `View`, `Content` conforms to `View`, and `Footer` is `EmptyView`.

Deprecated

Use init(content:header:) instead.

## Parameters 

`header`  

A view to use as the section’s header.

`content`  

The section’s content.

## See Also

### Deprecated symbols

init(footer: Footer, content: () -> Content)

Creates a section with a footer and the provided section content.

Deprecated

init(header: Parent, footer: Footer, content: () -> Content)

Creates a section with a header, footer, and the provided section content.

Deprecated

func collapsible(Bool) -> some View

Sets whether a section can be collapsed by the user.

Deprecated

