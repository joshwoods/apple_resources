

- SwiftUI
-  GlassBackgroundEffect 

Protocol

# GlassBackgroundEffect

A specification for the appearance of a glass background.

visionOS 2.4+

``` source
protocol GlassBackgroundEffect
```

## Topics

### Associated Types

associatedtype Body : GlassBackgroundEffect

The type of effect representing the body of this effect. When you create a custom effect, Swift infers this type from your implementation of the required makeBody(configuration:) method.

**Required**

### Instance Methods

func makeBody(configuration: Self.Configuration) -> Self.Body

Defines the effect produced by this effect.

**Required**

### Type Aliases

typealias Configuration

The configuration type passed to `makeBody(configuration:)`.

### Type Properties

static var automatic: AutomaticGlassBackgroundEffect

The default glass background effect, based on the glass’s context.

static var feathered: FeatheredGlassBackgroundEffect

A feathered background effect with default padding amount and default soft edge radiual size.

static var plate: PlateGlassBackgroundEffect

A plate glass background effect.

### Type Methods

static func feathered(padding: CGFloat, softEdgeRadius: CGFloat?) -> FeatheredGlassBackgroundEffect

A feathered background effect with custom padding and soft edge radius.

## Relationships

### Conforming Types

- AutomaticGlassBackgroundEffect
- FeatheredGlassBackgroundEffect
- PlateGlassBackgroundEffect

