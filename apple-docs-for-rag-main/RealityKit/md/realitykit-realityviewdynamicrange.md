

- RealityKit
-  RealityViewDynamicRange 

Structure

# RealityViewDynamicRange

Options that determine the state of high dynamic range rendering for virtual content.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct RealityViewDynamicRange
```

## Topics

### Setting the dynamic range

static var `default`: RealityViewDynamicRange

static var standard: RealityViewDynamicRange

### Protocol support

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

static func == (RealityViewDynamicRange, RealityViewDynamicRange) -> Bool

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

enum AntialiasingMode

The rendering technique used to smooth edges of virtual content.

struct Environment

A description of background, lighting, and acoustic properties for a view’s content.

struct RenderOptions

The available rendering options that you use to selectively disable certain rendering effects.

