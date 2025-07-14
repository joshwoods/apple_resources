

- UIKit
- UIAccessibilityReadingContent
-  accessibilityFrame(forLineNumber:) 

Instance Method

# accessibilityFrame(forLineNumber:)

Returns the onscreen frame associated with the specified line number.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityFrame(forLineNumber lineNumber: Int) -> CGRect
```

**Required**

## Parameters 

`lineNumber`  

The line number.

## Return Value

The frame in the receiver that contains the specified line number, in screen coordinates. By default, this method returns `CGRectZero`.

## Discussion

To determine the onscreen rectangle (or frame) of a line, you can use code such as the following:

- Swift
- Objective-C

```
let lineBounds: CGRect = // the bounds of the line in view space
let view: UIView = // the relevant view
return UIAccessibilityConvertFrameToScreenCoordinates(lineBounds, view)
```

```
CGRect lineBounds = // The bounds of the line in view space.
UIView *view = // The relevant view.
return UIAccessibilityConvertFrameToScreenCoordinates(lineBounds, view);
```

## See Also

### Related Documentation

static func convertToScreenCoordinates(CGRect, in: UIView) -> CGRect

Converts the specified rectangle from view coordinates to screen coordinates.

### Accessing the content on a page

func accessibilityLineNumber(for: CGPoint) -> Int

Returns the line number that contains the specified point.

**Required**

func accessibilityAttributedContent(forLineNumber: Int) -> NSAttributedString?

Returns the styled text associated with the specified line number.

func accessibilityContent(forLineNumber: Int) -> String?

Returns the text associated with the specified line number.

**Required**

func accessibilityAttributedPageContent() -> NSAttributedString?

Returns the styled text displayed on the current page.

func accessibilityPageContent() -> String?

Returns the text displayed on the current page.

**Required**

