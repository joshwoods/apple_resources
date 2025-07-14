

- UIKit
- UITextInputTraits
-  inlinePredictionType 

Instance Property

# inlinePredictionType

The behavior of inline text predictions for a text-entry area.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
optional var inlinePredictionType: UITextInlinePredictionType { get set }
```

## Discussion

This property controls whether system-provided text suggestions appear inline during typing. The default value is UITextInlinePredictionType.default.

If you use a UITextView or UITextField, set this property if you want to change the inline text prediction behavior. For example, you might want to turn off inline text predictions if your app provides its own text suggestions.

The following code turns off inline text predictions in a text view:

```
let textView = UITextView(frame: frame)
textView.inlinePredictionType = .no
```

## See Also

### Managing spelling and autocorrection

var autocapitalizationType: UITextAutocapitalizationType

The autocapitalization style for the text object.

enum UITextAutocapitalizationType

The autocapitalization behavior of a text-based view.

var autocorrectionType: UITextAutocorrectionType

The autocorrection style for the text object.

enum UITextAutocorrectionType

The autocorrection behavior of a text-based view.

var spellCheckingType: UITextSpellCheckingType

The spell-checking style for the text object.

enum UITextSpellCheckingType

The spell-checking behavior of a text-based view.

enum UITextInlinePredictionType

Constants that identify the behavior of inline text predictions for a text-entry area.

