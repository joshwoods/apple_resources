

- WebKit
-  DOMMouseEvent Deprecated

Class

# DOMMouseEvent

macOS 10.4–10.14Deprecated

``` source
class DOMMouseEvent
```

## Topics

### Instance Properties

var altKey: Bool

var button: Int16

var clientX: Int32

var clientY: Int32

var ctrlKey: Bool

var fromElement: DOMNode!

var metaKey: Bool

var offsetX: Int32

var offsetY: Int32

var relatedTarget: (any DOMEventTarget)!

var screenX: Int32

var screenY: Int32

var shiftKey: Bool

var toElement: DOMNode!

var x: Int32

var y: Int32

### Instance Methods

func initMouseEvent(String!, canBubble: Bool, cancelable: Bool, view: DOMAbstractView!, detail: Int32, screenX: Int32, screenY: Int32, clientX: Int32, clientY: Int32, ctrlKey: Bool, altKey: Bool, shiftKey: Bool, metaKey: Bool, button: UInt16, relatedTarget: (any DOMEventTarget)!)

## Relationships

### Inherits From

- DOMUIEvent

### Inherited By

- DOMWheelEvent

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

