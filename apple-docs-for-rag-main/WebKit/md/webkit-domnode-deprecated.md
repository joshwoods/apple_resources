

- WebKit
-  DOMNode Deprecated

Class

# DOMNode

macOS 10.4–10.14Deprecated

``` source
class DOMNode
```

## Topics

### Instance Properties

var attributes: DOMNamedNodeMap!

var baseURI: String!

var childNodes: DOMNodeList!

var firstChild: DOMNode!

var isContentEditable: Bool

var lastChild: DOMNode!

var localName: String!

var namespaceURI: String!

var nextSibling: DOMNode!

var nodeName: String!

var nodeType: UInt16

var nodeValue: String!

var ownerDocument: DOMDocument!

var parent: DOMNode!

var parentElement: DOMElement!

var prefix: String!

var previousSibling: DOMNode!

var textContent: String!

var webArchive: WebArchive!

A web archive of the content of the node and its children.

### Instance Methods

func appendChild(DOMNode!) -> DOMNode!

func boundingBox() -> NSRect

Returns a rectangle that bounds the onscreen rendering of the node.

func cloneNode(Bool) -> DOMNode!

func compareDocumentPosition(DOMNode!) -> UInt16

func contains(DOMNode!) -> Bool

func hasAttributes() -> Bool

func hasChildNodes() -> Bool

func insert(before: DOMNode!, refChild: DOMNode!) -> DOMNode!

func isDefaultNamespace(String!) -> Bool

func isEqualNode(DOMNode!) -> Bool

func isSameNode(DOMNode!) -> Bool

func isSupported(String!, version: String!) -> Bool

func lineBoxRects() -> [Any]!

Returns the rectangles that bound each line of text in the node.

func lookupNamespaceURI(String!) -> String!

func lookupPrefix(String!) -> String!

func normalize()

func removeChild(DOMNode!) -> DOMNode!

func replaceChild(DOMNode!, oldChild: DOMNode!) -> DOMNode!

## Relationships

### Inherits From

- DOMObject

### Inherited By

- DOMAttr
- DOMCharacterData
- DOMDocument
- DOMDocumentFragment
- DOMDocumentType
- DOMElement
- DOMEntity
- DOMEntityReference

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- DOMEventTarget
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

