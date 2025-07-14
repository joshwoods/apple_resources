

- Paravirtualized Graphics
- PGDisplay
-  newFrameEventHandler 

Instance Property

# newFrameEventHandler

A handler that the framework calls when the guest environment has a new frame to display.

Mac Catalyst 14.0+macOS 11.0+

``` source
var newFrameEventHandler: PGDisplayNewFrameEventHandler? { get }
```

**Required**

## See Also

### Inspecting the Display Handlers

var queue: dispatch_queue_t?

The queue that the framework uses when dispatching messages to any of the display’s registered handlers.

**Required**

var cursorGlyphHandler: PGDisplayCursorGlyphHandler?

A handler that the framework calls to change the cursor’s appearance.

**Required**

var cursorShowHandler: PGDisplayCursorShowHandler?

A handler that the framework calls to change the cursor’s visibility.

**Required**

var modeChangeHandler: PGDisplayModeChangeHandler?

A handler that the framework calls to change the virtual display’s graphics mode.

**Required**

