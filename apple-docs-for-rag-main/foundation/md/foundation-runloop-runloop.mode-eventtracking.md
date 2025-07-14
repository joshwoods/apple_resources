

- Foundation
- RunLoop
- RunLoop.Mode
-  eventTracking 

Type Property

# eventTracking

The mode set when tracking events modally, such as a mouse-dragging loop.

macOS 10.0+

``` source
static let eventTracking: RunLoop.Mode
```

## See Also

### System Run Loop Modes

static let common: RunLoop.Mode

A pseudo-mode that includes one or more other run loop modes.

static let `default`: RunLoop.Mode

The mode set to handle input sources other than connection objects.

static let modalPanel: RunLoop.Mode

The mode set when waiting for input from a modal panel, such as a save or open panel.

static let tracking: RunLoop.Mode

The mode set while tracking in controls takes place.

