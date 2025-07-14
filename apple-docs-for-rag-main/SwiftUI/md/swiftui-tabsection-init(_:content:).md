

- SwiftUI
- TabSection
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a section with the provided content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    _ titleKey: LocalizedStringKey,
    @TabContentBuilder content: () -> Content
) where Header == Text, Footer == EmptyView
```

Available when `Content` conforms to `TabContent` and `SelectionValue` conforms to `Hashable`.

Show all declarations

## Parameters 

`titleKey`  

The localized string key label for the section’s header.

`content`  

The section’s content.

## See Also

### Creating a tab section

init(content:)

Creates a section with the provided section content.

init(content:header:)

Creates a section with a header and the provided section content.

