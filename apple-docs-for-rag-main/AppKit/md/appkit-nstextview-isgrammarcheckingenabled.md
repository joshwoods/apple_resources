

- AppKit
- NSTextView
-  isGrammarCheckingEnabled 

Instance Property

# isGrammarCheckingEnabled

Enables and disables grammar checking.

macOS 10.5+

``` source
@MainActor
var isGrammarCheckingEnabled: Bool { get set }
```

## Discussion

If true, grammar checking is enabled; if false, it is disabled.

## See Also

### Working with the spelling checker

var isContinuousSpellCheckingEnabled: Bool

A Boolean value that indicates whether the receiver has continuous spell checking enabled.

var spellCheckerDocumentTag: Int

A tag identifying the text view’s text as a document for the spell checker server.

func toggleContinuousSpellChecking(Any?)

Toggles whether continuous spell checking is enabled for the receiver.

func toggleGrammarChecking(Any?)

Changes the state of grammar checking from enabled to disabled and vice versa.

func setSpellingState(Int, range: NSRange)

Sets the spelling state, which controls the display of the spelling and grammar indicators on the given text range.

