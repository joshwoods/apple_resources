

- BrowserEngineKit
- BETextInput
-  textInputView 

Instance Property

# textInputView

An affiliated view that provides a coordinate system for all geometric values in this protocol.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var textInputView: UIView { get }
```

**Required**

## Mentioned in 

Integrating custom browser text views with UIKit

Supporting extended text interactions

## See Also

### Geometry

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

func autoscroll(to: CGPoint)

Indicates autoscrolling has been triggered by a text interaction gesture.

**Required**

func cancelAutoscroll()

Indicates autoscrolling is complete.

**Required**

