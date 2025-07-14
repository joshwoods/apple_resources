

- AppKit
- NSTrackingArea
-  userInfo 

Instance Property

# userInfo

The dictionary containing the data associated with the receiver when it was created.

macOS 10.5+

``` source
var userInfo: [AnyHashable : Any]? { get }
```

## Discussion

You can obtain this dictionary per event in each mouseEntered(with:) and mouseExited(with:) method by querying the passed-in `NSEvent` object with `[[event trackingArea] userData]`.

## See Also

### Getting Object Attributes

var options: NSTrackingArea.Options

The options specified for the receiver.

var owner: AnyObject?

The object owning the receiver, which is the recipient of mouse-tracking, mouse-movement, and cursor-update messages.

var rect: NSRect

The rectangle defining the area encompassed by the receiver.

