

- WebKit
-  DOMRange Deprecated

Class

# DOMRange

macOS 10.4–10.14Deprecated

``` source
class DOMRange
```

## Topics

### Instance Properties

var collapsed: Bool

var commonAncestorContainer: DOMNode!

var endContainer: DOMNode!

var endOffset: Int32

var markupString: String!

A string in markup format corresponding to the content in the range.

var startContainer: DOMNode!

var startOffset: Int32

var text: String!

var webArchive: WebArchive!

A web archive of the content in the range.

### Instance Methods

func clone() -> DOMRange!

func cloneContents() -> DOMDocumentFragment!

func collapse(Bool)

func compare(DOMNode!) -> Int16

func compareBoundaryPoints(UInt16, sourceRange: DOMRange!) -> Int16

func comparePoint(DOMNode!, offset: Int32) -> Int16

func createContextualFragment(String!) -> DOMDocumentFragment!

func deleteContents()

func detach()

func extractContents() -> DOMDocumentFragment!

func insert(DOMNode!)

func intersects(DOMNode!) -> Bool

func isPoint(inRange: DOMNode!, offset: Int32) -> Bool

func select(DOMNode!)

func selectNodeContents(DOMNode!)

func setEnd(DOMNode!, offset: Int32)

func setEndAfter(DOMNode!)

func setEndBefore(DOMNode!)

func setStart(DOMNode!, offset: Int32)

func setStartAfter(DOMNode!)

func setStartBefore(DOMNode!)

func surroundContents(DOMNode!)

func toString() -> String!

## Relationships

### Inherits From

- DOMObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Document Object Model (DOM) APIs

class DOMAbstractViewDeprecated

class DOMAttrDeprecated

class DOMBlobDeprecated

class DOMCDATASectionDeprecated

class DOMCharacterDataDeprecated

class DOMCommentDeprecated

class DOMCounterDeprecated

class DOMCSSCharsetRuleDeprecated

class DOMCSSFontFaceRuleDeprecated

class DOMCSSImportRuleDeprecated

class DOMCSSMediaRuleDeprecated

class DOMCSSPageRuleDeprecated

class DOMCSSPrimitiveValueDeprecated

class DOMCSSRuleDeprecated

class DOMCSSRuleListDeprecated

