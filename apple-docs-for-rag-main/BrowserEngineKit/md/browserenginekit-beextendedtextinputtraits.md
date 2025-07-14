

- BrowserEngineKit
-  BEExtendedTextInputTraits 

Protocol

# BEExtendedTextInputTraits

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
protocol BEExtendedTextInputTraits : UITextInputTraits
```

## Topics

### Instance Properties

var insertionPointColor: UIColor?

Customizes the color of the text cursor at the insertion point

var isSingleLineDocument: Bool

Represents whether the active web input field is a single line document

var isTypingAdaptationEnabled: Bool

Disables the learning of new words and corrections and prevents their addition into the keyboard lexicon

var selectionHandleColor: UIColor?

Customizes the color of the selection handles

var selectionHighlightColor: UIColor?

Customizes the color of the selection highlight rect

## Relationships

### Inherits From

- NSObjectProtocol
- UITextInputTraits

## See Also

### Information about text

struct BEDirectionalTextRange

