

- SwiftUI
- MenuButton
-  init(\_:content:) Deprecated

Initializer

# init(\_:content:)

Creates a menu button with the specified localized title and content.

macOS 10.15–15.4Deprecated

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Text` and `Content` conforms to `View`.

Deprecated

Use Menu instead.

Show all declarations

## See Also

### Creating a menu button

init(label: Label, content: () -> Content)

Creates a menu button with the specified label and content.

Deprecated

