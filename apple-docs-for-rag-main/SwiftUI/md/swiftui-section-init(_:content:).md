

- SwiftUI
- Section
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a section with the provided section content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder content: () -> Content
)
```

Available when `Parent` is `Text`, `Content` conforms to `View`, and `Footer` is `EmptyView`.

Show all declarations

## Parameters 

`titleKey`  

The key for the section’s localized title, which describes the contents of the section.

`content`  

The section’s content.

## See Also

### Creating a section

init(content:)

Creates a section with the provided section content.

