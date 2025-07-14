

- AppKit
- NSTextView
-  insertCompletion(\_:forPartialWordRange:movement:isFinal:) 

Instance Method

# insertCompletion(\_:forPartialWordRange:movement:isFinal:)

Inserts the selected completion into the text at the appropriate location.

macOS

``` source
@MainActor
func insertCompletion(
    _ word: String,
    forPartialWordRange charRange: NSRange,
    movement: Int,
    isFinal flag: Bool
)
```

## Parameters 

`word`  

The text to insert, including the matched partial word and its potential completion.

`charRange`  

The range of characters of the matched partial word to be completed.

`movement`  

The direction of movement. For possible values see the NSText Constants section. This value allows subclasses to distinguish between canceling completion and selection by arrow keys, by return, by tab, or by other means such as clicking.

`flag`  

false while the user navigates through the potential text completions, true when a completion is definitively selected or cancelled and the original value is reinserted.

## Discussion

This method has two effects, text substitution and changing of the selection:

- It replaces the text between `charRange.start` and the current insertion point with `word`.

- If `flag` is false it changes the selection to be the last *n* characters of `word` where *n* is equal to `[word length]` minus `charRange.length`, that is, the potential completion.

- If `flag` is true it makes the selection empty and puts the insertion point just after `word`.

## See Also

### Performing text completion

func complete(Any?)

Invokes completion in a text view.

func completions(forPartialWordRange: NSRange, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>) -> [String]?

Returns an array of potential completions, in the order to be presented, representing possible word completions available from a partial word.

var rangeForUserCompletion: NSRange

The partial range from the most recent beginning of a word up to the insertion point.

