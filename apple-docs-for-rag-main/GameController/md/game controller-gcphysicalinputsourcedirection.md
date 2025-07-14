

- Game Controller
-  GCPhysicalInputSourceDirection 

Structure

# GCPhysicalInputSourceDirection

The directions that a physical input source involves.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct GCPhysicalInputSourceDirection
```

## Topics

### Directions

static var up: GCPhysicalInputSourceDirection

The physical input source contains a value for the up direction.

static var right: GCPhysicalInputSourceDirection

The physical input source supports the right direction.

static var down: GCPhysicalInputSourceDirection

The physical input source supports the down direction.

static var left: GCPhysicalInputSourceDirection

The physical input source supports the left direction.

### Initializers

init(rawValue: UInt)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting directions

var direction: GCPhysicalInputSourceDirection

The directional input, if any, that a physical input source involves.

**Required**

