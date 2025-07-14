

- BrowserEngineKit
- BETextDocumentRequest
-  BETextDocumentRequest.Options 

Structure

# BETextDocumentRequest.Options

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
struct Options
```

## Topics

### Initializers

init(rawValue: Int)

### Type Properties

static var attributedText: BETextDocumentRequest.Options

static var autocorrectedRanges: BETextDocumentRequest.Options

static var markedTextRects: BETextDocumentRequest.Options

static var text: BETextDocumentRequest.Options

static var textRects: BETextDocumentRequest.Options

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Replacements and AutoFill

class BEAutoFillTextSuggestion

class BETextAlternatives

class BETextDocumentContext

Information about the text surrounding a selection in a document.

class BETextDocumentRequest

class BETextSuggestion

A text suggestion to insert into a document.

struct BETextReplacementOptions

