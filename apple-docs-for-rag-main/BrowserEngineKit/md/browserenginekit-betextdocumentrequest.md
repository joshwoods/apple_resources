

- BrowserEngineKit
-  BETextDocumentRequest 

Class

# BETextDocumentRequest

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
class BETextDocumentRequest
```

## Topics

### Instance Properties

var granularityCount: Int

Represents the scope of the request as a count of granularity units specified in `surroundingGranularity`

var options: BETextDocumentRequest.Options

Represents the information that the system is requesting

var surroundingGranularity: UITextGranularity

Represents the granularity units for the scope of the request

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Replacements and AutoFill

class BEAutoFillTextSuggestion

class BETextAlternatives

class BETextDocumentContext

Information about the text surrounding a selection in a document.

struct Options

class BETextSuggestion

A text suggestion to insert into a document.

struct BETextReplacementOptions

