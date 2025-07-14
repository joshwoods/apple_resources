

- SwiftUI
-  Section 

Structure

# Section

A container view that you can use to add hierarchy within certain views.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Section
```

## Mentioned in 

Grouping data with lazy stack views

Suggesting search terms

Displaying data in lists

## Overview

Use `Section` instances in views like List, Picker, and Form to organize content into separate sections. Each section has custom content that you provide on a per-instance basis. You can also provide headers and footers for each section.

### Collapsible sections

Create sections that expand and collapse by using an initializer that accepts an `isExpanded` binding. A collapsible section in a List that uses the sidebar style shows a disclosure indicator next to the section’s header. Tapping on the disclosure indicator toggles the appearance of the section’s content.

Note

Not all contexts provide a default control to trigger collapse or expansion.

## Topics

### Creating a section

init(content:)

Creates a section with the provided section content.

init(_:content:)

Creates a section with the provided section content.

### Adding headers and footers

init(content:header:)

Creates a section with a header and the provided section content.

init(content: () -> Content, footer: () -> Footer)

Creates a section with a footer and the provided section content.

init(content: () -> Content, header: () -> Parent, footer: () -> Footer)

Creates a section with a header, footer, and the provided section content.

### Controlling collapsibility

init(_:isExpanded:content:)

Creates a section with the provided section content.

init(isExpanded:content:header:)

Creates a section with a header, the provided section content, and a binding representing the section’s expansion state.

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

func collapsible(Bool) -> some View

Sets whether a section can be collapsed by the user.

Deprecated

## Relationships

### Conforms To

- Copyable
- TableRowContent

  Conforms when `Parent` conforms to `TableRowContent`, `Content` conforms to `TableRowContent`, and `Footer` conforms to `TableRowContent`.

- View

  Conforms when `Parent` conforms to `View`, `Content` conforms to `View`, and `Footer` conforms to `View`.

## See Also

### Organizing views into sections

struct SectionCollection

An opaque collection representing the sections of view.

struct SectionConfiguration

Specifies the contents of a section.

