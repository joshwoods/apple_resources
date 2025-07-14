

- RealityKit
-  AntialiasingMode 

Enumeration

# AntialiasingMode

The rendering technique used to smooth edges of virtual content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum AntialiasingMode
```

## Topics

### Setting the antialiasing mode

case multisample4X

Multisampling renders each pixel multiple times and combines the results, creating a higher quality image at a performance cost proportional to the number of samples used.

case none

Do not apply any technique to smooth jagged edges.

### Protocol support

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

static func == (AntialiasingMode, AntialiasingMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Visual environment adjustments

struct RealityViewEnvironment

A struct that determines the background and default lighting properties for a reality view.

struct RealityViewRenderingEffects

A struct for enabling and disabling rendering effects for RealityKit content.

struct RealityViewRenderingEffectMode

A mode that determines whether a rendering effect is enabled or disabled.

struct RealityViewDynamicRange

Options that determine the state of high dynamic range rendering for virtual content.

struct Environment

A description of background, lighting, and acoustic properties for a view’s content.

struct RenderOptions

The available rendering options that you use to selectively disable certain rendering effects.

