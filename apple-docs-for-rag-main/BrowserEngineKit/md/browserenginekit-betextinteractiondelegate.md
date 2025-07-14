

- BrowserEngineKit
-  BETextInteractionDelegate 

Protocol

# BETextInteractionDelegate

A set of methods that informs you about selection changes in text views.

iOS 17.4+iPadOS 17.4+macOStvOS 17.4+visionOS 1.1+

``` source
protocol BETextInteractionDelegate
```

## Topics

### Text selection changes

func systemWillChangeSelection(for: BETextInteraction)

Invoked by the system when the selection is about to change in the document.

**Required**

func systemDidChangeSelection(for: BETextInteraction)

Invoked by the system when the selection is about to change in the document.

**Required**

## See Also

### Interaction responses

class BETextInteraction

An interaction you add to a text view to support extended text gestures.

protocol BEResponderEditActions

A set of methods that defines extended interactions in browser text views.

enum BEGestureType

protocol BEResponderEditActions

A set of methods that defines extended interactions in browser text views.

