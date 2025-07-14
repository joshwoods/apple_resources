

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
-  LayerRenderer.Frame.Timing 

Structure

# LayerRenderer.Frame.Timing

A type that stores information about a frame’s encoding, rendering, and presentation deadlines.

visionOS 1.0+

``` source
struct Timing
```

## Overview

Before you start drawing your frame’s content, call predictTiming() to retrieve the frame’s timing information. That function returns the latest predicted values for you to use during planning. After you retrieve the LayerRenderer.Drawable type for the frame, get the timing information from the drawable instead using frameTiming.

## Topics

### Updating the frame contents

var optimalInputTime: LayerRenderer.Clock.Instant

The optimal time to start the frame submission process.

### Rendering the frame

var renderingDeadline: LayerRenderer.Clock.Instant

The time at which you must finish all work for the specified frame.

### Displaying the frame

var presentationTime: LayerRenderer.Clock.Instant

The time at which the system displays the frame onscreen.

### Creating the timing details

init()

### Instance Properties

var trackableAnchorTime: LayerRenderer.Clock.Instant

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Getting timing information

func predictTiming() -> LayerRenderer.Frame.Timing?

Computes and returns the predicted timing information for the frame.

