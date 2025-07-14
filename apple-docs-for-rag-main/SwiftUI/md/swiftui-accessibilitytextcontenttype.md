

- SwiftUI
-  AccessibilityTextContentType 

Structure

# AccessibilityTextContentType

Textual context that assistive technologies can use to improve the presentation of spoken text.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AccessibilityTextContentType
```

## Overview

Use an `AccessibilityTextContentType` value when setting the accessibility text content type of a view using the accessibilityTextContentType(_:) modifier.

## Topics

### Getting content types

static let console: AccessibilityTextContentType

A type that represents text used for input, like in the Terminal app.

static let fileSystem: AccessibilityTextContentType

A type that represents text used by a file browser, like in the Finder app in macOS.

static let messaging: AccessibilityTextContentType

A type that represents text used in a message, like in the Messages app.

static let narrative: AccessibilityTextContentType

A type that represents text used in a story or poem, like in the Books app.

static let plain: AccessibilityTextContentType

A type that represents generic text that has no specific type.

static let sourceCode: AccessibilityTextContentType

A type that represents text used in source code, like in Swift Playgrounds.

static let spreadsheet: AccessibilityTextContentType

A type that represents text used in a grid of data, like in the Numbers app.

static let wordProcessing: AccessibilityTextContentType

A type that represents text used in a document, like in the Pages app.

## Relationships

### Conforms To

- Sendable

## See Also

### Describing content

func accessibilityTextContentType(AccessibilityTextContentType) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets an accessibility text content type.

func accessibilityHeading(AccessibilityHeadingLevel) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the accessibility level of this heading.

enum AccessibilityHeadingLevel

The hierarchy of a heading in relation other headings.

