

- Paravirtualized Graphics
- PGDisplay
-  cursorShowHandler 

Instance Property

# cursorShowHandler

A handler that the framework calls to change the cursor’s visibility.

Mac Catalyst 14.0+macOS 11.0+

``` source
var cursorShowHandler: PGDisplayCursorShowHandler? { get }
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

var modeChangeHandler: PGDisplayModeChangeHandler?

A handler that the framework calls to change the virtual display’s graphics mode.

**Required**

var newFrameEventHandler: PGDisplayNewFrameEventHandler?

A handler that the framework calls when the guest environment has a new frame to display.

**Required**

