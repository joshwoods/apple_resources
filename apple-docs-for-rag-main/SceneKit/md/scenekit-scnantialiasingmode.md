

- SceneKit
-  SCNAntialiasingMode 

Enumeration

# SCNAntialiasingMode

Modes for antialiased rendering of the view’s scene, used by the SCNView property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNAntialiasingMode
```

## Topics

### Constants

case none

Disables antialiased rendering.

case multisampling2X

Enables multisample antialiasing, with two samples per screen pixel.

case multisampling4X

Enables multisample antialiasing, with four samples per screen pixel.

case multisampling8X

Enables multisample antialiasing, with eight samples per screen pixel.

case multisampling16X

Enables multisample antialiasing, with sixteen samples per screen pixel.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring a View

var backgroundColor: NSColor

The background color of the view.

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

var rendersContinuously: Bool

A Boolean value that determines whether the view always renders at its preferred frame rate or only when its visible content changes.

var antialiasingMode: SCNAntialiasingMode

The antialiasing mode used for rendering the view’s scene.

