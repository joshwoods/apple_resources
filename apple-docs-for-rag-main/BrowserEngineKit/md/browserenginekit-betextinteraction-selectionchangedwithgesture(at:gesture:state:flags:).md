

- BrowserEngineKit
- BETextInteraction
-  selectionChangedWithGesture(at:gesture:state:flags:) 

Instance Method

# selectionChangedWithGesture(at:gesture:state:flags:)

Notifies the system that the text view changed its selection.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func selectionChangedWithGesture(
    at point: CGPoint,
    gesture gestureType: BEGestureType,
    state gestureState: UIGestureRecognizer.State,
    flags: BESelectionFlags
)
```

## Overview

Call this method when your browser text view receives updateCurrentSelection(to:from:in:).

## See Also

### Text selection

var delegate: (any BETextInteractionDelegate)?

A delegate object that the interaction notifies when the system changes the text selection.

protocol BETextInteractionDelegate

A set of methods that informs you about selection changes in text views.

var textSelectionDisplayInteraction: UITextSelectionDisplayInteraction

An interaction that manages the system’s text-selection UI.

func selectionBoundaryAdjusted(to: CGPoint, touchPhase: BESelectionTouchPhase, flags: BESelectionFlags)

Notifies the system after the text view adjusts its selection.

