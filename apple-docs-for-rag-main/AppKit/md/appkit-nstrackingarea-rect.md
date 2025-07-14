

- AppKit
- NSTrackingArea
-  rect 

Instance Property

# rect

The rectangle defining the area encompassed by the receiver.

macOS 10.5+

``` source
var rect: NSRect { get }
```

## Discussion

The rectangle is specified in the local coordinate system of the associated view. If the inVisibleRect option is specified, the receiver is automatically synchronized with changes in the view’s visible area (visibleRect) and the value of this property is ignored.

## See Also

### Getting Object Attributes

var options: NSTrackingArea.Options

The options specified for the receiver.

var owner: AnyObject?

The object owning the receiver, which is the recipient of mouse-tracking, mouse-movement, and cursor-update messages.

var userInfo: [AnyHashable : Any]?

The dictionary containing the data associated with the receiver when it was created.

