

- BrowserEngineKit
-  BETextInputDelegate 

Protocol

# BETextInputDelegate

A delegate protocol that a browser text view uses to notify the text system of changes.

iOS 17.4+iPadOS 17.4+macOStvOS 17.4+visionOS 1.1+

``` source
protocol BETextInputDelegate
```

## Mentioned in 

Integrating custom browser text views with UIKit

## Overview

You don’t conform to `BETextInputDelegate` in your classes, or implement its methods. The operating system creates objects that conform to this protocol and sets them as the asyncInputDelegate on your browser’s custom text views.

## Topics

### Text selection

func selectionWillChange(for: any BETextInput)

Tells the system when the selection is about to change in the document.

**Required**

func selectionDidChange(for: any BETextInput)

Tells the system when the selection has changed in the document.

**Required**

### Deferring actions to the text system

func shouldDeferEventHandlingToSystem(for: any BETextInput, context: BEKeyEntryContext) -> Bool

Defers the key event to the system and returns whether the key event was handled.

**Required**

func textInput(any BETextInput, deferReplaceTextActionToSystem: Any)

Defers a replace text action to the ssytem.

**Required**

### Providing completion suggestions

func textInput(any BETextInput, setCandidateSuggestions: [BETextSuggestion]?)

Provides text suggestions to the system.

**Required**

### Removing stored context information

func invalidateTextEntryContext(for: any BETextInput)

Tells the system the text entry context has changed and that text entry UI’s need to be refreshed.

**Required**

## See Also

### Custom text views

Integrating custom browser text views with UIKit

Process keyboard interactions asynchronously in your iOS browser app’s text view.

Supporting extended text interactions

Share content, add replacement shortcuts, and perform other rich actions in browser text views.

protocol BETextInput

A protocol to which text views conform to asynchronously integrate with the text system.

