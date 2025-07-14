

- UIKit
- UIAccessibilityReadingContent
-  accessibilityLineNumber(for:) 

Instance Method

# accessibilityLineNumber(for:)

Returns the line number that contains the specified point.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityLineNumber(for point: CGPoint) -> Int
```

**Required**

## Parameters 

`point`  

A point within the bounds of the receiver’s view space, in screen coordinates. That is, a point for which `[self pointInside:point withEvent:event] == YES`.

## Return Value

The line number that contains the specified point or `NSNotFound` if the point indicates an empty area within the receiver’s rectangle. By default, this method returns `NSNotFound`.

## Discussion

This method is called only when `point` is within the bounds of the view or element.

## See Also

### Related Documentation

static func convertToScreenCoordinates(CGRect, in: UIView) -> CGRect

Converts the specified rectangle from view coordinates to screen coordinates.

### Accessing the content on a page

func accessibilityAttributedContent(forLineNumber: Int) -> NSAttributedString?

Returns the styled text associated with the specified line number.

func accessibilityContent(forLineNumber: Int) -> String?

Returns the text associated with the specified line number.

**Required**

func accessibilityFrame(forLineNumber: Int) -> CGRect

Returns the onscreen frame associated with the specified line number.

**Required**

func accessibilityAttributedPageContent() -> NSAttributedString?

Returns the styled text displayed on the current page.

func accessibilityPageContent() -> String?

Returns the text displayed on the current page.

**Required**

