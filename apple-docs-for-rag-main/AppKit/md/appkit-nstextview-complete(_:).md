

- AppKit
- NSTextView
-  complete(\_:) 

Instance Method

# complete(\_:)

Invokes completion in a text view.

macOS

``` source
@MainActor
func complete(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message. May be `nil`.

## Discussion

By default invoked using the F5 key, this method provides users with a choice of completions for the word currently being typed. May be invoked programmatically if autocompletion is desired by a client of the text system. You can change the key invoking this method using the text system’s key bindings mechanism; see “Text System Defaults and Key Bindings” for an explanation of the procedure.

The delegate may replace or modify the list of possible completions by implementing textView(_:completions:forPartialWordRange:indexOfSelectedItem:). Subclasses can control the list by overriding completions(forPartialWordRange:indexOfSelectedItem:).

## See Also

### Performing text completion

func completions(forPartialWordRange: NSRange, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>) -> [String]?

Returns an array of potential completions, in the order to be presented, representing possible word completions available from a partial word.

func insertCompletion(String, forPartialWordRange: NSRange, movement: Int, isFinal: Bool)

Inserts the selected completion into the text at the appropriate location.

var rangeForUserCompletion: NSRange

The partial range from the most recent beginning of a word up to the insertion point.

