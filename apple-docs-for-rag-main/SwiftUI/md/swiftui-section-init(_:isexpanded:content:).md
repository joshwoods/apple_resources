

- SwiftUI
- Section
-  init(\_:isExpanded:content:) 

Initializer

# init(\_:isExpanded:content:)

Creates a section with the provided section content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    _ titleKey: LocalizedStringKey,
    isExpanded: Binding,
    @ViewBuilder content: () -> Content
)
```

Available when `Parent` is `Text`, `Content` conforms to `View`, and `Footer` is `EmptyView`.

Show all declarations

## Parameters 

`titleKey`  

The key for the section’s localized title, which describes the contents of the section.

`isExpanded`  

A binding to a Boolean value that determines the section’s expansion state (expanded or collapsed).

`content`  

The section’s content.

## See Also

### Controlling collapsibility

init(isExpanded:content:header:)

Creates a section with a header, the provided section content, and a binding representing the section’s expansion state.

