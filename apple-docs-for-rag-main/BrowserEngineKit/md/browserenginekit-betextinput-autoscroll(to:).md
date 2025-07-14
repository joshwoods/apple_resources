

- BrowserEngineKit
- BETextInput
-  autoscroll(to:) 

Instance Method

# autoscroll(to:)

Indicates autoscrolling has been triggered by a text interaction gesture.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func autoscroll(to point: CGPoint)
```

**Required**

## Parameters 

`point`  

The location to which to autoscroll, in the coordinate system of your view’s textInputView.

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

Called repeatedly during range adjustment gestures, or when placing the text cursor.

The given point is in the coordinate space of the `textInputView`.

Indicates that a text gesture initiated autoscrolling.

## Overview

The text system calls the method repeatedly when a gesture requires the text view to scroll, for example, when a person adjusts the text selection range, or places the text cursor. The text system sends cancelAutoscroll() when there are no further updates.

## See Also

### Geometry

var textInputView: UIView

An affiliated view that provides a coordinate system for all geometric values in this protocol.

**Required**

var textFirstRect: CGRect

Returns a rect representing the bounds of the first line of marked text, if marked text is set.

**Required**

var textLastRect: CGRect

Returns a rect representing the bounds of the last line of marked text, if marked text is set.

**Required**

var unobscuredContentRect: CGRect

Rect used to place UI (such as selection handles) in a location that isn’t obscurred by app UI.

**Required**

var unscaledView: UIView

View representing the web content that is agnostic of zoom state. Used to draw zoom agnostic system UI elements, such as the selection handles

**Required**

var selectionClipRect: CGRect

Rect representing the bounds of editable elements, used to ensure and UI don’t overflow outside them

**Required**

func cancelAutoscroll()

Indicates autoscrolling is complete.

**Required**

