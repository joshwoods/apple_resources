

- BrowserEngineKit
- BETextInput
-  setBaseWritingDirection(\_:for:) 

Instance Method

# setBaseWritingDirection(\_:for:)

Sets the base writing direction for a specified range of text in a document.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func setBaseWritingDirection(
    _ writingDirection: NSWritingDirection,
    for range: UITextRange
)
```

**Required**

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

Informs the text view of the writing direction for a given range of text.

- writingDirection: Whether the writing direction is left-to-right, right-to-left, or the natural direction for the current script.

- range: The range in the text view’s document for which the writing direction applies.

## See Also

### Handling text input

var isEditable: Bool

Reflects the ability to modify text

**Required**

func handleKeyEntry(BEKeyEntry, completionHandler: (BEKeyEntry, Bool) -> Void)

Accepts key-entry events from the text system for the text view to process.

**Required**

func shiftKeyStateChanged(fromState: BEKeyModifierFlags, toState: BEKeyModifierFlags)

Indicates a transition in shift state

**Required**

func text(in: UITextRange) -> String?

Returns the text in the specified range.

**Required**

func offset(from: UITextPosition, to: UITextPosition) -> Int

Returns the number of UTF-16 characters between one text position and another text position.

**Required**

func delete(in: UITextStorageDirection, to: UITextGranularity)

Deletes text by the specified direction and granularity. Current supported combinations include:

**Required**

