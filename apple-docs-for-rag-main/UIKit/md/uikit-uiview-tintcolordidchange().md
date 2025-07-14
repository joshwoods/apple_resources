

- UIKit
- UIView
-  tintColorDidChange() 

Instance Method

# tintColorDidChange()

Called by the system when the tint color property changes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func tintColorDidChange()
```

## Discussion

The system calls this method on a view when your code changes the value of the tintColor property on that view. In addition, the system calls this method on a subview that inherits a changed interaction tint color.

In your implementation, refresh the view rendering as needed.

## See Also

### Related Documentation

var tintColor: UIColor!

The first nondefault tint color value in the view’s hierarchy, ascending from and starting with the view itself.

### Drawing and updating the view

func draw(CGRect)

Draws the view’s image within the passed-in rectangle.

func setNeedsDisplay()

Marks the receiver’s entire bounds rectangle as needing to be redrawn.

func setNeedsDisplay(CGRect)

Marks the specified rectangle of the receiver as needing to be redrawn.

var contentScaleFactor: CGFloat

The scale factor applied to the view.

