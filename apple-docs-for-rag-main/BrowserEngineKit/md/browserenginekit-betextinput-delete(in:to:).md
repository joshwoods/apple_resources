

- BrowserEngineKit
- BETextInput
-  delete(in:to:) 

Instance Method

# delete(in:to:)

Deletes text by the specified direction and granularity. Current supported combinations include:

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func delete(
    in direction: UITextStorageDirection,
    to granularity: UITextGranularity
)
```

**Required**

## Parameters 

`direction`  

The direction in which to delete text, relative to the base writing direction.

`granularity`  

The amount of text to delete.

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

Character backward = delete character forward = delete-forward word backward = option + delete word forward = option + delete-forward line end = cmd + delete line start = cmd + delete-forward paragraph end = ctrl + K paragraph start = ctrl + fn + K

(On Apple keyboards, the delete-forward key is a combination of fn + delete)

Deletes the specified amount of text.

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

func setBaseWritingDirection(NSWritingDirection, for: UITextRange)

Sets the base writing direction for a specified range of text in a document.

**Required**

