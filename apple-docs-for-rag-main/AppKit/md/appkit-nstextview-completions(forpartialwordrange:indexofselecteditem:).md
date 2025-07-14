

- AppKit
- NSTextView
-  completions(forPartialWordRange:indexOfSelectedItem:) 

Instance Method

# completions(forPartialWordRange:indexOfSelectedItem:)

Returns an array of potential completions, in the order to be presented, representing possible word completions available from a partial word.

macOS

``` source
@MainActor
func completions(
    forPartialWordRange charRange: NSRange,
    indexOfSelectedItem index: UnsafeMutablePointer
) -> [String]?
```

## Parameters 

`charRange`  

The range of characters of the matched partial word to be completed.

`index`  

On return, optionally set to the completion that should be initially selected. The default is 0, and –1 indicates no selection.

## Return Value

An array of potential completions, in the order to be presented, representing possible word completions available from a partial word at `charRange`. Returning `nil` or a zero-length array suppresses completion.

## Discussion

May be overridden by subclasses to modify or override the list of possible completions.

This method should call the delegate method textView(_:completions:forPartialWordRange:indexOfSelectedItem:) if the delegate implements such a method.

## See Also

### Performing text completion

func complete(Any?)

Invokes completion in a text view.

func insertCompletion(String, forPartialWordRange: NSRange, movement: Int, isFinal: Bool)

Inserts the selected completion into the text at the appropriate location.

var rangeForUserCompletion: NSRange

The partial range from the most recent beginning of a word up to the insertion point.

