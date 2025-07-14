

- AppKit
- NSTextView
-  rangeForUserCompletion 

Instance Property

# rangeForUserCompletion

The partial range from the most recent beginning of a word up to the insertion point.

macOS

``` source
@MainActor
var rangeForUserCompletion: NSRange { get }
```

## Discussion

This value is intended to be used for the range argument in the text completion methods such as completions(forPartialWordRange:indexOfSelectedItem:).

## See Also

### Performing text completion

func complete(Any?)

Invokes completion in a text view.

func completions(forPartialWordRange: NSRange, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>) -> [String]?

Returns an array of potential completions, in the order to be presented, representing possible word completions available from a partial word.

func insertCompletion(String, forPartialWordRange: NSRange, movement: Int, isFinal: Bool)

Inserts the selected completion into the text at the appropriate location.

