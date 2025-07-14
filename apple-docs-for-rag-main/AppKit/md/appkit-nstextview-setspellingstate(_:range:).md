

- AppKit
- NSTextView
-  setSpellingState(\_:range:) 

Instance Method

# setSpellingState(\_:range:)

Sets the spelling state, which controls the display of the spelling and grammar indicators on the given text range.

macOS 10.5+

``` source
@MainActor
func setSpellingState(
    _ value: Int,
    range charRange: NSRange
)
```

## Parameters 

`value`  

The spelling state value to set. Possible values, for the temporary attribute on the layout manager using the key NSSpellingStateAttributeName, are:

- NSSpellingStateSpellingFlag to highlight spelling issues.

- NSSpellingStateGrammarFlag to highlight grammar issues.

`charRange`  

The character range over which to set the given spelling state.

## Discussion

May be called or overridden to control setting of spelling and grammar indicators on text, used to highlight portions of the text that are flagged for spelling or grammar issues.

## See Also

### Working with the spelling checker

var isContinuousSpellCheckingEnabled: Bool

A Boolean value that indicates whether the receiver has continuous spell checking enabled.

var spellCheckerDocumentTag: Int

A tag identifying the text view’s text as a document for the spell checker server.

func toggleContinuousSpellChecking(Any?)

Toggles whether continuous spell checking is enabled for the receiver.

var isGrammarCheckingEnabled: Bool

Enables and disables grammar checking.

func toggleGrammarChecking(Any?)

Changes the state of grammar checking from enabled to disabled and vice versa.

