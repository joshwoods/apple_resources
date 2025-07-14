

- WebKit
-  DOMEventTarget Deprecated

Protocol

# DOMEventTarget

macOS 10.4–10.14Deprecated

``` source
protocol DOMEventTarget : NSCopying, NSObjectProtocol
```

## Topics

### Instance Methods

func addEventListener(String!, listener: (any DOMEventListener)!, useCapture: Bool)

**Required**

func dispatchEvent(DOMEvent!) -> Bool

**Required**

func removeEventListener(String!, listener: (any DOMEventListener)!, useCapture: Bool)

**Required**

## Relationships

### Inherits From

- NSCopying
- NSObjectProtocol

### Conforming Types

- DOMAttr
- DOMCDATASection
- DOMCharacterData
- DOMComment
- DOMDocument
- DOMDocumentFragment
- DOMDocumentType
- DOMElement
- DOMEntity
- DOMEntityReference
- DOMHTMLAnchorElement
- DOMHTMLAppletElement
- DOMHTMLAreaElement
- DOMHTMLBRElement
- DOMHTMLBaseElement
- DOMHTMLBaseFontElement
- DOMHTMLBodyElement
- DOMHTMLButtonElement
- DOMHTMLDListElement
- DOMHTMLDirectoryElement
- DOMHTMLDivElement
- DOMHTMLDocument
- DOMHTMLElement
- DOMHTMLEmbedElement
- DOMHTMLFieldSetElement
- DOMHTMLFontElement
- DOMHTMLFormElement
- DOMHTMLFrameElement
- DOMHTMLFrameSetElement
- DOMHTMLHRElement
- DOMHTMLHeadElement
- DOMHTMLHeadingElement
- DOMHTMLHtmlElement
- DOMHTMLIFrameElement
- DOMHTMLImageElement
- DOMHTMLInputElement
- DOMHTMLLIElement
- DOMHTMLLabelElement
- DOMHTMLLegendElement
- DOMHTMLLinkElement
- DOMHTMLMapElement
- DOMHTMLMarqueeElement
- DOMHTMLMenuElement
- DOMHTMLMetaElement
- DOMHTMLModElement
- DOMHTMLOListElement
- DOMHTMLObjectElement
- DOMHTMLOptGroupElement
- DOMHTMLOptionElement
- DOMHTMLParagraphElement
- DOMHTMLParamElement
- DOMHTMLPreElement
- DOMHTMLQuoteElement
- DOMHTMLScriptElement
- DOMHTMLSelectElement
- DOMHTMLStyleElement
- DOMHTMLTableCaptionElement
- DOMHTMLTableCellElement
- DOMHTMLTableColElement
- DOMHTMLTableElement
- DOMHTMLTableRowElement
- DOMHTMLTableSectionElement
- DOMHTMLTextAreaElement
- DOMHTMLTitleElement
- DOMHTMLUListElement
- DOMNode
- DOMProcessingInstruction
- DOMText

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

