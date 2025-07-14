

- WebKit
- Deprecated Symbols
- Document Object Models API (Legacy)
-  DOMNode Additions 

API Collection

# DOMNode Additions

Additions to the `DOMNode` class help convert the structured nodes of DOM content into a rich web-viewable form.

## Topics

### Creating archives

var webArchive: WebArchive!

A web archive of the content of the node and its children.

### Obtaining layout rectangles

func boundingBox() -> NSRect

Returns a rectangle that bounds the onscreen rendering of the node.

func lineBoxRects() -> [Any]!

Returns the rectangles that bound each line of text in the node.

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

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

