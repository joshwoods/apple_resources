

- SwiftUI
-  AccessibilityHeadingLevel 

Enumeration

# AccessibilityHeadingLevel

The hierarchy of a heading in relation other headings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum AccessibilityHeadingLevel
```

## Overview

Assistive technologies can use this to improve a users navigation through multiple headings. When users navigate through top level headings they expect the content for each heading to be unrelated.

For example, you can categorize a list of available products into sections, like Fruits and Vegetables. With only top level headings, this list requires no heading hierarchy, and you use the AccessibilityHeadingLevel.unspecified heading level. On the other hand, if sections contain subsections, like if the Fruits section has subsections for varieties of Apples, Pears, and so on, you apply the AccessibilityHeadingLevel.h1 level to Fruits and Vegetables, and the AccessibilityHeadingLevel.h2 level to Apples and Pears.

Except for AccessibilityHeadingLevel.h1, be sure to precede all leveled headings by another heading with a level that’s one less.

## Topics

### Getting the heading level

case h1

Level 1 heading.

case h2

Level 2 heading.

case h3

Level 3 heading.

case h4

Level 4 heading.

case h5

Level 5 heading.

case h6

Level 6 heading.

case unspecified

A heading without a hierarchy.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Describing content

func accessibilityTextContentType(AccessibilityTextContentType) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets an accessibility text content type.

func accessibilityHeading(AccessibilityHeadingLevel) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the accessibility level of this heading.

struct AccessibilityTextContentType

Textual context that assistive technologies can use to improve the presentation of spoken text.

