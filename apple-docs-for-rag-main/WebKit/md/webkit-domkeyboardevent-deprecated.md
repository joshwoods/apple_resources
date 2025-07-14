

- WebKit
-  DOMKeyboardEvent Deprecated

Class

# DOMKeyboardEvent

macOS 10.5–10.14Deprecated

``` source
class DOMKeyboardEvent
```

## Topics

### Instance Properties

var altGraphKey: Bool

var altKey: Bool

var charCode: Int32

var ctrlKey: Bool

var keyCode: Int32

var keyIdentifier: String!

var location: UInt32

var metaKey: Bool

var shiftKey: Bool

### Instance Methods

func getModifierState(String!) -> Bool

func initKeyboardEvent(String!, canBubble: Bool, cancelable: Bool, view: DOMAbstractView!, keyIdentifier: String!, location: UInt32, ctrlKey: Bool, altKey: Bool, shiftKey: Bool, metaKey: Bool)

func initKeyboardEvent(String!, canBubble: Bool, cancelable: Bool, view: DOMAbstractView!, keyIdentifier: String!, location: UInt32, ctrlKey: Bool, altKey: Bool, shiftKey: Bool, metaKey: Bool, altGraphKey: Bool)

## Relationships

### Inherits From

- DOMUIEvent

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

