

- AppKit
- NSTextView
-  spellCheckerDocumentTag 

Instance Property

# spellCheckerDocumentTag

A tag identifying the text view’s text as a document for the spell checker server.

macOS

``` source
@MainActor
var spellCheckerDocumentTag: Int { get }
```

## Discussion

The document tag is obtained by sending a uniqueSpellDocumentTag() message to the spell server the first time this method is invoked for a particular group of text views. See the NSSpellCheckerand NSSpellServerclass specifications for more information on how this tag is used.

## See Also

### Working with the spelling checker

var isContinuousSpellCheckingEnabled: Bool

A Boolean value that indicates whether the receiver has continuous spell checking enabled.

func toggleContinuousSpellChecking(Any?)

Toggles whether continuous spell checking is enabled for the receiver.

var isGrammarCheckingEnabled: Bool

Enables and disables grammar checking.

func toggleGrammarChecking(Any?)

Changes the state of grammar checking from enabled to disabled and vice versa.

func setSpellingState(Int, range: NSRange)

Sets the spelling state, which controls the display of the spelling and grammar indicators on the given text range.

