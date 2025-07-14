

- BrowserEngineKit
- BETextInput
-  textInteractionGesture(\_:shouldBeginAt:) 

Instance Method

# textInteractionGesture(\_:shouldBeginAt:)

Returns whether a gesture with the given `gestureType` should begin for the given `point`

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func textInteractionGesture(
    _ gestureType: BEGestureType,
    shouldBeginAt point: CGPoint
) -> Bool
```

**Required**

## Parameters 

`gestureType`  

The type of gesture that’s possibly beginning.

`point`  

The location of the gesture in the text view.

## Return Value

`true` to permit the text system to proceed with the gesture; `false` otherwise.

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

Returns whether a gesture at the given point in the view needs to begin.

## See Also

### Handling text gestures

func updateCurrentSelection(to: CGPoint, from: BEGestureType, in: UIGestureRecognizer.State)

Indicates the `point` the text interaction gesture is tracking has changed

**Required**

func setSelection(from: CGPoint, to: CGPoint, gesture: BEGestureType, state: UIGestureRecognizer.State)

Notifies the text view that its selection needs to change to the text between the given points.

**Required**

func adjustSelectionBoundary(to: CGPoint, touchPhase: BESelectionTouchPhase, baseIsStart: Bool, flags: BESelectionFlags)

Adjusts the selection’s start or end boundary specified by `boundaryIsStart` to the `point`

**Required**

