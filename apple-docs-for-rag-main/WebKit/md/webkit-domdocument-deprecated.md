

- WebKit
-  DOMDocument Deprecated

Class

# DOMDocument

macOS 10.4–10.14Deprecated

``` source
class DOMDocument
```

## Topics

### Instance Properties

var activeElement: DOMElement!

var anchors: DOMHTMLCollection!

var applets: DOMHTMLCollection!

var body: DOMHTMLElement!

var characterSet: String!

var charset: String!

var cookie: String!

var defaultCharset: String!

var defaultView: DOMAbstractView!

var doctype: DOMDocumentType!

var documentElement: DOMElement!

var documentURI: String!

var domain: String!

var forms: DOMHTMLCollection!

var images: DOMHTMLCollection!

var implementation: DOMImplementation!

var inputEncoding: String!

var lastModified: String!

var links: DOMHTMLCollection!

var preferredStylesheetSet: String!

var readyState: String!

var referrer: String!

var selectedStylesheetSet: String!

var styleSheets: DOMStyleSheetList!

var title: String!

var url: String!

var webFrame: WebFrame!

The web frame associated with the DOM document.

var xmlEncoding: String!

var xmlStandalone: Bool

var xmlVersion: String!

### Instance Methods

func adoptNode(DOMNode!) -> DOMNode!

func createAttribute(String!) -> DOMAttr!

func createAttributeNS(String!, qualifiedName: String!) -> DOMAttr!

func createCDATASection(String!) -> DOMCDATASection!

func createCSSStyleDeclaration() -> DOMCSSStyleDeclaration!

func createComment(String!) -> DOMComment!

func createDocumentFragment() -> DOMDocumentFragment!

func createElement(String!) -> DOMElement!

func createElementNS(String!, qualifiedName: String!) -> DOMElement!

func createEntityReference(String!) -> DOMEntityReference!

func createEvent(String!) -> DOMEvent!

func createExpression(String!, resolver: (any DOMXPathNSResolver)!) -> DOMXPathExpression!

func createNSResolver(DOMNode!) -> (any DOMXPathNSResolver)!

func createNodeIterator(DOMNode!, whatToShow: UInt32, filter: (any DOMNodeFilter)!, expandEntityReferences: Bool) -> DOMNodeIterator!

func createProcessingInstruction(String!, data: String!) -> DOMProcessingInstruction!

func createRange() -> DOMRange!

func createTextNode(String!) -> DOMText!

func createTreeWalker(DOMNode!, whatToShow: UInt32, filter: (any DOMNodeFilter)!, expandEntityReferences: Bool) -> DOMTreeWalker!

func element(fromPoint: Int32, y: Int32) -> DOMElement!

func evaluate(String!, contextNode: DOMNode!, resolver: (any DOMXPathNSResolver)!, type: UInt16, in: DOMXPathResult!) -> DOMXPathResult!

func execCommand(String!) -> Bool

func execCommand(String!, userInterface: Bool) -> Bool

func execCommand(String!, userInterface: Bool, value: String!) -> Bool

func getComputedStyle(DOMElement!, pseudoElement: String!) -> DOMCSSStyleDeclaration!

func getElementById(String!) -> DOMElement!

func getElementsByClassName(String!) -> DOMNodeList!

func getElementsByName(String!) -> DOMNodeList!

func getElementsByTagName(String!) -> DOMNodeList!

func getElementsByTagNameNS(String!, localName: String!) -> DOMNodeList!

func getMatchedCSSRules(DOMElement!, pseudoElement: String!) -> DOMCSSRuleList!

func getMatchedCSSRules(DOMElement!, pseudoElement: String!, authorOnly: Bool) -> DOMCSSRuleList!

func getOverrideStyle(DOMElement!, pseudoElement: String!) -> DOMCSSStyleDeclaration!

func hasFocus() -> Bool

func `import`(DOMNode!, deep: Bool) -> DOMNode!

func queryCommandEnabled(String!) -> Bool

func queryCommandIndeterm(String!) -> Bool

func queryCommandState(String!) -> Bool

func queryCommandSupported(String!) -> Bool

func queryCommandValue(String!) -> String!

func querySelector(String!) -> DOMElement!

func querySelectorAll(String!) -> DOMNodeList!

func url(withAttributeString: String!) -> URL!

Constructs a URL given an attribute string.

func webkitCancelFullScreen()

## Relationships

### Inherits From

- DOMNode

### Inherited By

- DOMHTMLDocument

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

