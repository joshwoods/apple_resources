

- UIKit
- UIDictationPhrase
-  alternativeInterpretations 

Instance Property

# alternativeInterpretations

An array of alternative textual interpretations of a dictated phrase.

iOS 5.1+iPadOS 5.1+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var alternativeInterpretations: [String]? { get }
```

## Discussion

If the system determines only one textual interpretation of a dictated phrase, the value of this property is `nil`. If there’s more than one interpretation, this property contains an array of strings, with the first being most likely interpretation and the last being the least likely.

## See Also

### Obtaining textual interpretations of spoken text

var text: String

The most likely textual interpretation of a dictated phrase.

