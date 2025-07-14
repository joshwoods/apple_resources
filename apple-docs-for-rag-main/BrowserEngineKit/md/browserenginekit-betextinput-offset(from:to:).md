

- BrowserEngineKit
- BETextInput
-  offset(from:to:) 

Instance Method

# offset(from:to:)

Returns the number of UTF-16 characters between one text position and another text position.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func offset(
    from: UITextPosition,
    to toPosition: UITextPosition
) -> Int
```

**Required**

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

Returns the distance between two positions in the text view’s text.

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

func setBaseWritingDirection(NSWritingDirection, for: UITextRange)

Sets the base writing direction for a specified range of text in a document.

**Required**

func delete(in: UITextStorageDirection, to: UITextGranularity)

Deletes text by the specified direction and granularity. Current supported combinations include:

**Required**

