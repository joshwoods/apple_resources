

- Core Image
-  CIRenderDestinationAlphaMode 

Enumeration

# CIRenderDestinationAlphaMode

Different ways of representing alpha.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum CIRenderDestinationAlphaMode : UInt, @unchecked Sendable
```

## Topics

### Enumeration Cases

case none

Designates a destination with no alpha compositing.

case premultiplied

Designates a destination that expects premultiplied alpha values.

case unpremultiplied

Designates a destination that expects non-premultiplied alpha values.

## Relationships

### Conforms To

- Sendable

## See Also

### Custom Render Destination

Generating an animation with a Core Image Render Destination

Animate a filtered image to a Metal view in a SwiftUI app using a Core Image Render Destination.

class CIRenderDestination

A specification for configuring all attributes of a render task's destination and issuing asynchronous render tasks.

class CIRenderInfo

An encapsulation of a render task's timing, passes, and pixels processed.

class CIRenderTask

A single render task issued in conjunction with CIRenderDestination.

