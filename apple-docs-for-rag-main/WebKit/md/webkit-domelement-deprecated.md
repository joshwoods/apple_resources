

- WebKit
-  DOMElement Deprecated

Class

# DOMElement

macOS 10.4–10.14Deprecated

``` source
class DOMElement
```

## Topics

### Instance Properties

var childElementCount: UInt32

var className: String!

var clientHeight: Int32

var clientLeft: Int32

var clientTop: Int32

var clientWidth: Int32

var firstElementChild: DOMElement!

var innerHTML: String!

var innerText: String!

var lastElementChild: DOMElement!

var nextElementSibling: DOMElement!

var offsetHeight: Int32

var offsetLeft: Int32

var offsetParent: DOMElement!

var offsetTop: Int32

var offsetWidth: Int32

var outerHTML: String!

var previousElementSibling: DOMElement!

var scrollHeight: Int32

var scrollLeft: Int32

var scrollTop: Int32

var scrollWidth: Int32

var style: DOMCSSStyleDeclaration!

var tagName: String!

### Instance Methods

func blur()

func focus()

func getAttribute(String!) -> String!

func getAttributeNS(String!, localName: String!) -> String!

func getAttributeNode(String!) -> DOMAttr!

func getAttributeNodeNS(String!, localName: String!) -> DOMAttr!

func getElementsByClassName(String!) -> DOMNodeList!

func getElementsByTagName(String!) -> DOMNodeList!

func getElementsByTagNameNS(String!, localName: String!) -> DOMNodeList!

func hasAttribute(String!) -> Bool

func hasAttributeNS(String!, localName: String!) -> Bool

func image() -> NSImage!

Returns an image associated with the receiver.

func querySelector(String!) -> DOMElement!

func querySelectorAll(String!) -> DOMNodeList!

func removeAttribute(String!)

func removeAttributeNS(String!, localName: String!)

func removeAttributeNode(DOMAttr!) -> DOMAttr!

func scroll(byLines: Int32)

func scroll(byPages: Int32)

func scroll(intoView: Bool)

func scroll(intoViewIfNeeded: Bool)

func setAttribute(String!, value: String!)

func setAttributeNS(String!, qualifiedName: String!, value: String!)

func setAttributeNode(DOMAttr!) -> DOMAttr!

func setAttributeNodeNS(DOMAttr!) -> DOMAttr!

func webkitRequestFullScreen(UInt16)

## Relationships

### Inherits From

- DOMNode

### Inherited By

- DOMHTMLElement

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

