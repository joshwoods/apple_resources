

- BrowserEngineKit
- BETextInput
-  updateCurrentSelection(to:from:in:) 

Instance Method

# updateCurrentSelection(to:from:in:)

Indicates the `point` the text interaction gesture is tracking has changed

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func updateCurrentSelection(
    to point: CGPoint,
    from gestureType: BEGestureType,
    in state: UIGestureRecognizer.State
)
```

**Required**

## Parameters 

`point`  

The new location of the gesture.

`gestureType`  

The type of gesture the system is tracking.

`state`  

The state of the gesture.

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

Indicate to the system the change was handled by invoking: -\[BETextInteraction selectionChangedWithGestureAtPoint:gesture:state:flags:\]

Indicates that the point at which the system is tracking an active gesture changed.

## Overview

When you receive this method, call selectionChangedWithGesture(at:gesture:state:flags:) to notify the system that your text view handled the update.

## See Also

### Handling text gestures

func setSelection(from: CGPoint, to: CGPoint, gesture: BEGestureType, state: UIGestureRecognizer.State)

Notifies the text view that its selection needs to change to the text between the given points.

**Required**

func adjustSelectionBoundary(to: CGPoint, touchPhase: BESelectionTouchPhase, baseIsStart: Bool, flags: BESelectionFlags)

Adjusts the selection’s start or end boundary specified by `boundaryIsStart` to the `point`

**Required**

func textInteractionGesture(BEGestureType, shouldBeginAt: CGPoint) -> Bool

Returns whether a gesture with the given `gestureType` should begin for the given `point`

**Required**

