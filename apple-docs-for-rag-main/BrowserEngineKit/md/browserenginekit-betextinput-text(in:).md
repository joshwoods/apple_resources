

- BrowserEngineKit
- BETextInput
-  text(in:) 

Instance Method

# text(in:)

Returns the text in the specified range.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func text(in range: UITextRange) -> String?
```

**Required**

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

Returns the text in a browser’s text view in the given range.

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

func offset(from: UITextPosition, to: UITextPosition) -> Int

Returns the number of UTF-16 characters between one text position and another text position.

**Required**

func setBaseWritingDirection(NSWritingDirection, for: UITextRange)

Sets the base writing direction for a specified range of text in a document.

**Required**

func delete(in: UITextStorageDirection, to: UITextGranularity)

Deletes text by the specified direction and granularity. Current supported combinations include:

**Required**

