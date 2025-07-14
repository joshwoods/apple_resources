

- AppKit
- NSEvent
- NSEvent.EventTypeMask
-  smartMagnify 

Type Property

# smartMagnify

A mask for smart-zoom gesture events.

macOS 10.8+

``` source
static var smartMagnify: NSEvent.EventTypeMask { get }
```

## Discussion

In response to this event, magnify the content appropriately for your app. For example, you might zoom in on a specific paragraph or image.

## See Also

### Getting Touch Events

static var beginGesture: NSEvent.EventTypeMask

A mask for begin-gesture events.

static var endGesture: NSEvent.EventTypeMask

A mask for end-gesture events.

static var magnify: NSEvent.EventTypeMask

A mask for magnify-gesture events.

static var swipe: NSEvent.EventTypeMask

A mask for swipe-gesture events.

static var rotate: NSEvent.EventTypeMask

A mask for rotate-gesture events.

static var gesture: NSEvent.EventTypeMask

A mask for generic gesture events.

static var directTouch: NSEvent.EventTypeMask

A mask for touch events.

static var tabletPoint: NSEvent.EventTypeMask

A mask for tablet-point events.

static var tabletProximity: NSEvent.EventTypeMask

A mask for tablet-proximity events.

static var pressure: NSEvent.EventTypeMask

A mask for pressure-change events.

