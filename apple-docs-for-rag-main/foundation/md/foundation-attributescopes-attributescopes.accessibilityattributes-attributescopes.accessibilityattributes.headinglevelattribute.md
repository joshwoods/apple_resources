

- Foundation
- AttributeScopes
- AttributeScopes.AccessibilityAttributes
-  AttributeScopes.AccessibilityAttributes.HeadingLevelAttribute 

Enumeration

# AttributeScopes.AccessibilityAttributes.HeadingLevelAttribute

An attribute for the level of this heading.

FoundationAccessibilityiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum HeadingLevelAttribute
```

## Overview

Assistive technologies can use this property to improve navigation and describe the level number of levels AttributeScopes.AccessibilityAttributes.HeadingLevelAttribute.HeadingLevel.h1 through AttributeScopes.AccessibilityAttributes.HeadingLevelAttribute.HeadingLevel.h6 alongside the text.

For example, you can rank sections within UI using a heading level. The most important section is marked withAttributeScopes.AccessibilityAttributes.HeadingLevelAttribute.HeadingLevel.h1. Nested sections can use subsequent heading levels. For unranked headings, use AttributeScopes.AccessibilityAttributes.HeadingLevelAttribute.HeadingLevel.unspecified.

## Topics

### Enumerations

enum HeadingLevel

The hierarchy of a heading in relation other headings.

## Relationships

### Conforms To

- AttributedStringKey
- BitwiseCopyable
- Copyable
- DecodableAttributedStringKey
- EncodableAttributedStringKey
- MarkdownDecodableAttributedStringKey
- ObjectiveCConvertibleAttributedStringKey
- Sendable

