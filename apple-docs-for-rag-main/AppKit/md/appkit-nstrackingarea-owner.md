

- AppKit
- NSTrackingArea
-  owner 

Instance Property

# owner

The object owning the receiver, which is the recipient of mouse-tracking, mouse-movement, and cursor-update messages.

macOS 10.5+

``` source
weak var owner: AnyObject? { get }
```

## See Also

### Getting Object Attributes

var options: NSTrackingArea.Options

The options specified for the receiver.

var rect: NSRect

The rectangle defining the area encompassed by the receiver.

var userInfo: [AnyHashable : Any]?

The dictionary containing the data associated with the receiver when it was created.

