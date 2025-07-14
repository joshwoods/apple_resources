

- BrowserEngineKit
- BETextInput
-  shiftKeyStateChanged(fromState:toState:) 

Instance Method

# shiftKeyStateChanged(fromState:toState:)

Indicates a transition in shift state

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func shiftKeyStateChanged(
    fromState oldState: BEKeyModifierFlags,
    toState newState: BEKeyModifierFlags
)
```

**Required**

## Parameters 

`oldState`  

The previous shift-key state.

`newState`  

The new shift-key state.

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

Indicates that a person has pressed or released a Shift key, or toggled the caps lock state.

## See Also

### Handling text input

var isEditable: Bool

Reflects the ability to modify text

**Required**

func handleKeyEntry(BEKeyEntry, completionHandler: (BEKeyEntry, Bool) -> Void)

Accepts key-entry events from the text system for the text view to process.

**Required**

func text(in: UITextRange) -> String?

Returns the text in the specified range.

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

