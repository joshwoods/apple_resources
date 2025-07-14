

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
-  LayerRenderer.Drawable.State 

Enumeration

# LayerRenderer.Drawable.State

The state of ownership for the drawable.

visionOS 1.0+

``` source
enum State
```

## Overview

Use these constants to determine whether the drawable is ready for you to use. When the drawable is in the LayerRenderer.Drawable.State.rendering state, you can begin drawing. Other states indicate the drawable is either busy or not assigned to a frame.

## Topics

### Getting the states

case available

A drawable that’s not in use and ready for assignment to a frame.

case presenting

A drawable that the compositor is currently displaying.

case rendering

A drawable that’s assigned to a frame and ready to accept your drawing commands.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the state machine

var state: LayerRenderer.Drawable.State

The current operational state of a drawable instance.

