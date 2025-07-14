

- UIKit
-  UIAccessibilityTextualContext 

Structure

# UIAccessibilityTextualContext

Constants that describe a named context that helps identify and classify the type of text inside an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct UIAccessibilityTextualContext
```

## Topics

### Constants

static let console: UIAccessibilityTextualContext

A constant that indicates the text appears in a console context.

static let fileSystem: UIAccessibilityTextualContext

A constant that indicates the text appears in a file-system context.

static let messaging: UIAccessibilityTextualContext

A constant that indicates the text appears in a messaging context.

static let narrative: UIAccessibilityTextualContext

A constant that indicates the text appears in a narrative speech context.

static let sourceCode: UIAccessibilityTextualContext

A constant that indicates the text appears in a source-code context.

static let spreadsheet: UIAccessibilityTextualContext

A constant that indicates the text appears in a spreadsheet context.

static let wordProcessing: UIAccessibilityTextualContext

A constant that indicates the text appears in a word-processing context.

### Initializers

init(String)

Creates a textual context.

init(rawValue: String)

Creates a textual context with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Behaviors

UIAccessibilityFocus

An informal protocol that provides a way to determine whether an assistive app, such as VoiceOver, has focus on an accessible element.

protocol UIAccessibilityIdentification

Methods that associate a unique identifier with elements in your user interface.

protocol UIAccessibilityReadingContent

Methods to implement for an object that represents content that users read, such as a book or an article.

protocol UIAccessibilityContentSizeCategoryImageAdjusting

Methods to determine when to adjust images for different content size categories.

