

- SwiftUI
- Section
-  collapsible(\_:) Deprecated

Instance Method

# collapsible(\_:)

Sets whether a section can be collapsed by the user.

macOS 10.15–15.4Deprecated

``` source
func collapsible(_ collapsible: Bool) -> some View
```

Available when `Parent` conforms to `View`, `Content` conforms to `View`, and `Footer` conforms to `View`.

Deprecated

To disable collapsibility in macOS 14 and later, use one of the Section initializers that lacks collapsibility.

## Discussion

This modifier only applies to sections in List views that have the sidebar style.

## See Also

### Deprecated symbols

init(header: Parent, content: () -> Content)

Creates a section with a header and the provided section content.

Deprecated

init(footer: Footer, content: () -> Content)

Creates a section with a footer and the provided section content.

Deprecated

init(header: Parent, footer: Footer, content: () -> Content)

Creates a section with a header, footer, and the provided section content.

Deprecated

