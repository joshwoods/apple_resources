

- BrowserEngineKit
- BETextInput
-  setSelection(from:to:gesture:state:) 

Instance Method

# setSelection(from:to:gesture:state:)

Notifies the text view that its selection needs to change to the text between the given points.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func setSelection(
    from: CGPoint,
    to: CGPoint,
    gesture: BEGestureType,
    state: UIGestureRecognizer.State
)
```

**Required**

## Parameters 

`from`  

The start of the selected region.

`to`  

The end of the selected region.

`gesture`  

The gesture that changes the selection.

`state`  

The state of the gesture.

## Mentioned in 

Integrating custom browser text views with UIKit

## See Also

### Handling text gestures

func updateCurrentSelection(to: CGPoint, from: BEGestureType, in: UIGestureRecognizer.State)

Indicates the `point` the text interaction gesture is tracking has changed

**Required**

func adjustSelectionBoundary(to: CGPoint, touchPhase: BESelectionTouchPhase, baseIsStart: Bool, flags: BESelectionFlags)

Adjusts the selection’s start or end boundary specified by `boundaryIsStart` to the `point`

**Required**

func textInteractionGesture(BEGestureType, shouldBeginAt: CGPoint) -> Bool

Returns whether a gesture with the given `gestureType` should begin for the given `point`

**Required**

