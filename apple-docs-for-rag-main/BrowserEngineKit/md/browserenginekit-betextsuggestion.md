

- BrowserEngineKit
-  BETextSuggestion 

Class

# BETextSuggestion

A text suggestion to insert into a document.

iOS 17.4+iPadOS 17.4+macOStvOS 17.4+visionOS 1.1+

``` source
class BETextSuggestion
```

## Mentioned in 

Integrating custom browser text views with UIKit

## Overview

You typically don’t create instances of `BETextSuggestion`. The system supplies them to your browser text view’s insert(_:) method to suggest text insertions, for example AutoFill suggestions.

## Topics

### Creating a text suggestion

init(inputText: String)

Initializes a new text suggestion with the given input text.

### Getting the suggested text

var inputText: String

Text that will be inserted into the document when the user chooses the suggestion.

## Relationships

### Inherits From

- NSObject

### Inherited By

- BEAutoFillTextSuggestion

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

class BETextDocumentRequest

struct Options

struct BETextReplacementOptions

