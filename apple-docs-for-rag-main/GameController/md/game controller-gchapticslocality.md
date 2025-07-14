

- Game Controller
-  GCHapticsLocality 

Structure

# GCHapticsLocality

The location of one or more haptics actuators on a game controller.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct GCHapticsLocality
```

## Discussion

Use this symbol to specify the location of the actuators when creating a haptic engine.

## Topics

### Localities

static let `default`: GCHapticsLocality

The default location of a haptics actuator on a game controller.

static let all: GCHapticsLocality

All locations of haptics actuators on a game controller.

static let handles: GCHapticsLocality

All handles on a game controller.

static let leftHandle: GCHapticsLocality

The left handle on a game controller.

static let rightHandle: GCHapticsLocality

The right handle on a game controller.

static let triggers: GCHapticsLocality

All triggers on a game controller.

static let leftTrigger: GCHapticsLocality

The left trigger on a game controller.

static let rightTrigger: GCHapticsLocality

The right trigger on a game controller.

### Initializers

init(rawValue: String)

Creates a locality structure with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the localities

var supportedLocalities: Set&lt;GCHapticsLocality>

The locations of haptic actuators on the device.

