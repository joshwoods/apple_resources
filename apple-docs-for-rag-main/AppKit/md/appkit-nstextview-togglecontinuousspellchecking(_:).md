

- AppKit
- NSTextView
-  toggleContinuousSpellChecking(\_:) 

Instance Method

# toggleContinuousSpellChecking(\_:)

Toggles whether continuous spell checking is enabled for the receiver.

macOS

``` source
@MainActor
func toggleContinuousSpellChecking(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message; may be `nil`.

## See Also

### Working with the spelling checker

var isContinuousSpellCheckingEnabled: Bool

A Boolean value that indicates whether the receiver has continuous spell checking enabled.

var spellCheckerDocumentTag: Int

A tag identifying the text view’s text as a document for the spell checker server.

var isGrammarCheckingEnabled: Bool

Enables and disables grammar checking.

func toggleGrammarChecking(Any?)

Changes the state of grammar checking from enabled to disabled and vice versa.

func setSpellingState(Int, range: NSRange)

Sets the spelling state, which controls the display of the spelling and grammar indicators on the given text range.

