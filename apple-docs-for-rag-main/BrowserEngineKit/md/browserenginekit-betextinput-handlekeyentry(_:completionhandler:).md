

- BrowserEngineKit
- BETextInput
-  handleKeyEntry(\_:completionHandler:) 

Instance Method

# handleKeyEntry(\_:completionHandler:)

Accepts key-entry events from the text system for the text view to process.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func handleKeyEntry(
    _ entry: BEKeyEntry,
    completionHandler: @escaping (BEKeyEntry, Bool) -> Void
)
```

``` source
func handleKeyEntry(_ entry: BEKeyEntry) async -> (BEKeyEntry, Bool)
```

**Required**

## Parameters 

`entry`  

The keyboard event delivered by the operating system.

`completionHandler`  

A block that you call to indicate whether your text view handled the event.

## Mentioned in 

Integrating custom browser text views with UIKit

## Overview

Implement this method to receive keyboard events from the operating system. If you handle the `entry` in code, call the completion handler with `true` as the second parameter. Otherwise, call the completion handler with `false` as the second argument, and call the delegate’s shouldDeferEventHandlingToSystem(for:context:) method. In either case, pass the `entry` you received as the first parameter to the completion handler.

The operating system delivers events on a serial queue, so call the completion handler after your view processes an event to allow the operating system to send a subsequent event.

## See Also

### Handling text input

var isEditable: Bool

Reflects the ability to modify text

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

func delete(in: UITextStorageDirection, to: UITextGranularity)

Deletes text by the specified direction and granularity. Current supported combinations include:

**Required**

