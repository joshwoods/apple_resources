

- AppKit
- NSTrackingArea
-  options 

Instance Property

# options

The options specified for the receiver.

macOS 10.5+

``` source
var options: NSTrackingArea.Options { get }
```

## Discussion

The options for an `NSTrackingArea` object are specified when the object is created.

## See Also

### Getting Object Attributes

var owner: AnyObject?

The object owning the receiver, which is the recipient of mouse-tracking, mouse-movement, and cursor-update messages.

var rect: NSRect

The rectangle defining the area encompassed by the receiver.

var userInfo: [AnyHashable : Any]?

The dictionary containing the data associated with the receiver when it was created.

