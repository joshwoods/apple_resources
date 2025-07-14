

- Paravirtualized Graphics
-  PGDisplayDescriptor 

Class

# PGDisplayDescriptor

A descriptor for a virtual display.

Mac Catalyst 14.0+macOS 11.0+

``` source
class PGDisplayDescriptor
```

## Topics

### Specifying the Display Properties

var name: String?

The display’s name as seen in the guest operating environment.

var sizeInMillimeters: NSSize

The size in millimeters of the virtual display.

### Setting the Dispatch Queue

var queue: dispatch_queue_t?

The queue that the framework uses when dispatching messages to any of the display’s registered handlers.

### Managing Cursor Events

var cursorGlyphHandler: PGDisplayCursorGlyphHandler?

A handler that the framework calls to change the cursor’s appearance.

var cursorShowHandler: PGDisplayCursorShowHandler?

A handler that the framework calls to change the cursor’s visibility.

typealias PGDisplayCursorGlyphHandler

The block signature for a routine that handles changes to the cursor’s appearance.

typealias PGDisplayCursorShowHandler

The block signature for a routine that handles changes to the cursor’s visibility.

### Handling Mode Changes

var modeChangeHandler: PGDisplayModeChangeHandler?

A handler that the framework calls to change the virtual display’s graphics mode.

typealias PGDisplayModeChangeHandler

The block signature for a routine that handles changes to the display’s graphics mode.

### Handling Frame Events

var newFrameEventHandler: PGDisplayNewFrameEventHandler?

A handler that the framework calls when the guest environment has a new frame to display.

typealias PGDisplayNewFrameEventHandler

The block signature for a routine that handles frame updates from the guest.

### Instance Properties

var cursorMoveHandler: PGDisplayCursorMoveHandler?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Displays

protocol PGDisplay

An object that provides display functionality to the guest operating system in a way that the host-side virtual machine app can intercept.

class PGDisplayMode

A description of a supported display mode.

struct PGDisplayCoord_t

Coordinates that describe sizes or offsets within a 2D array of pixels.

