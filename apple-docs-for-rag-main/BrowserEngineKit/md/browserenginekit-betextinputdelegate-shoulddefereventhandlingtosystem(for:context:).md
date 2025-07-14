

- BrowserEngineKit
- BETextInputDelegate
-  shouldDeferEventHandlingToSystem(for:context:) 

Instance Method

# shouldDeferEventHandlingToSystem(for:context:)

Defers the key event to the system and returns whether the key event was handled.

iOS 17.4+iPadOS 17.4+macOStvOS 17.4+visionOS 1.1+

``` source
func shouldDeferEventHandlingToSystem(
    for textInput: any BETextInput,
    context keyEventContext: BEKeyEntryContext
) -> Bool
```

**Required**

## Parameters 

`textInput`  

The view for which the system needs to take over event handling.

`keyEventContext`  

Information about the key event and the document it targets.

## Return Value

`true` if the system handles the key event; `false` otherwise.

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

For example, the system will handle key events for character insertions, deletions, key commands, and more.

Notify the text system that your web browser’s custom text view isn’t handling key events.

## Overview

Call this method on your asyncInputDelegate when your BETextInput view doesn’t handle a key event, and you pass `false` to the `completionHandler` for handleKeyEntry(_:completionHandler:).

## See Also

### Deferring actions to the text system

func textInput(any BETextInput, deferReplaceTextActionToSystem: Any)

Defers a replace text action to the ssytem.

**Required**

