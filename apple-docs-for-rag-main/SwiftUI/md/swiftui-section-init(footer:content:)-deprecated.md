

- SwiftUI
- Section
-  init(footer:content:) Deprecated

Initializer

# init(footer:content:)

Creates a section with a footer and the provided section content.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
init(
    footer: Footer,
    @ViewBuilder content: () -> Content
)
```

Available when `Parent` is `EmptyView`, `Content` conforms to `View`, and `Footer` conforms to `View`.

Deprecated

Use init(content:footer:) instead.

## Parameters 

`footer`  

A view to use as the section’s footer.

`content`  

The section’s content.

## See Also

### Deprecated symbols

init(header: Parent, content: () -> Content)

Creates a section with a header and the provided section content.

Deprecated

init(header: Parent, footer: Footer, content: () -> Content)

Creates a section with a header, footer, and the provided section content.

Deprecated

func collapsible(Bool) -> some View

Sets whether a section can be collapsed by the user.

Deprecated

