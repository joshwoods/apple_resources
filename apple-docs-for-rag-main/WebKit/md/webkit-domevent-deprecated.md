

- WebKit
-  DOMEvent Deprecated

Class

# DOMEvent

macOS 10.4–10.14Deprecated

``` source
class DOMEvent
```

## Topics

### Instance Properties

var bubbles: Bool

var cancelBubble: Bool

var cancelable: Bool

var currentTarget: (any DOMEventTarget)!

var eventPhase: UInt16

var returnValue: Bool

var srcElement: (any DOMEventTarget)!

var target: (any DOMEventTarget)!

var timeStamp: DOMTimeStamp

var type: String!

### Instance Methods

func initEvent(String!, canBubbleArg: Bool, cancelableArg: Bool)

func preventDefault()

func stopPropagation()

## Relationships

### Inherits From

- DOMObject

### Inherited By

- DOMMutationEvent
- DOMOverflowEvent
- DOMProgressEvent
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

