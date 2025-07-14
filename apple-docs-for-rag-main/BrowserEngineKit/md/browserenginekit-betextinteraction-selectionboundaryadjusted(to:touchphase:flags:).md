

- BrowserEngineKit
- BETextInteraction
-  selectionBoundaryAdjusted(to:touchPhase:flags:) 

Instance Method

# selectionBoundaryAdjusted(to:touchPhase:flags:)

Notifies the system after the text view adjusts its selection.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func selectionBoundaryAdjusted(
    to point: CGPoint,
    touchPhase touch: BESelectionTouchPhase,
    flags: BESelectionFlags
)
```

## Overview

Call this method when your browser text view receives adjustSelectionBoundary(to:touchPhase:baseIsStart:flags:).

## See Also

### Text selection

var delegate: (any BETextInteractionDelegate)?

A delegate object that the interaction notifies when the system changes the text selection.

protocol BETextInteractionDelegate

A set of methods that informs you about selection changes in text views.

var textSelectionDisplayInteraction: UITextSelectionDisplayInteraction

An interaction that manages the system’s text-selection UI.

func selectionChangedWithGesture(at: CGPoint, gesture: BEGestureType, state: UIGestureRecognizer.State, flags: BESelectionFlags)

Notifies the system that the text view changed its selection.

