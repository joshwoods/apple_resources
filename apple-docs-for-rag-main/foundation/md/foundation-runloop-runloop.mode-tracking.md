

- Foundation
- RunLoop
- RunLoop.Mode
-  tracking 

Type Property

# tracking

The mode set while tracking in controls takes place.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+

``` source
static let tracking: RunLoop.Mode
```

## Discussion

You can use this mode to add timers that fire during tracking.

## See Also

### System Run Loop Modes

static let common: RunLoop.Mode

A pseudo-mode that includes one or more other run loop modes.

static let `default`: RunLoop.Mode

The mode set to handle input sources other than connection objects.

static let eventTracking: RunLoop.Mode

The mode set when tracking events modally, such as a mouse-dragging loop.

static let modalPanel: RunLoop.Mode

The mode set when waiting for input from a modal panel, such as a save or open panel.

