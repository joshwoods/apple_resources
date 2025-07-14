

- Foundation
-  InlinePresentationIntent 

Structure

# InlinePresentationIntent

A type that defines presentation intent for runs of characters for traits like emphasis, strikethrough, and code voice.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct InlinePresentationIntent
```

## Topics

### Getting inline presentation types

static var code: InlinePresentationIntent

An intent that represents a code voice presentation.

static var emphasized: InlinePresentationIntent

An intent that represents an emphasized presentation.

static var lineBreak: InlinePresentationIntent

An intent that represents a line break.

static var softBreak: InlinePresentationIntent

An intent that represents a soft line break.

static var strikethrough: InlinePresentationIntent

An intent that represents a strikethrough presentation.

static var stronglyEmphasized: InlinePresentationIntent

An intent that represents a strongly emphasized presentation.

static var inlineHTML: InlinePresentationIntent

An intent that represents an inline HTML presentation.

static var blockHTML: InlinePresentationIntent

An intent that represents a block HTML presentation.

### Creating Inline Presentation Intents

init(rawValue: UInt)

static var code: InlinePresentationIntent

An intent that represents a code voice presentation.

static var emphasized: InlinePresentationIntent

An intent that represents an emphasized presentation.

static var lineBreak: InlinePresentationIntent

An intent that represents a line break.

static var softBreak: InlinePresentationIntent

An intent that represents a soft line break.

static var strikethrough: InlinePresentationIntent

An intent that represents a strikethrough presentation.

static var stronglyEmphasized: InlinePresentationIntent

An intent that represents a strongly emphasized presentation.

static var inlineHTML: InlinePresentationIntent

An intent that represents an inline HTML presentation.

static var blockHTML: InlinePresentationIntent

An intent that represents a block HTML presentation.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

