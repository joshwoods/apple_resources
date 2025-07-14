

- Core Animation
-  CAEmitterCell 

Class

# CAEmitterCell

The definition of a particle emitted by a particle layer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
class CAEmitterCell
```

## Overview

The CAEmitterCell class represents one source of particles being emitted by a CAEmitterLayer object. An emitter cell defines the direction and properties of the emitted particles. Emitter cells can have an array of sub-cells, which lets the particles themselves emit particles.

## Topics

### Providing Emitter Cell Content

var contents: Any?

An object that provides the contents of the layer. Animatable.

var contentsRect: CGRect

A rectangle (in the unit coordinate space) that specifies the portion of contents that the receiver should draw. Animatable.

var emitterCells: [CAEmitterCell]?

An optional array containing the sub-cells of this cell.

### Setting Emitter Cell Visual Attributes

var isEnabled: Bool

A Boolean value indicating whether or not cells from this emitter are rendered.

var color: CGColor?

The color of each emitted object. Animatable.

var redRange: Float

The amount by which the red color component of the cell can vary. Animatable.

var greenRange: Float

The amount by which the green color component of the cell can vary. Animatable.

var blueRange: Float

The amount by which the blue color component of the cell can vary. Animatable.

var alphaRange: Float

The amount by which the alpha component of the cell can vary. Animatable.

var redSpeed: Float

The speed, in seconds, at which the red color component changes over the lifetime of the cell. Animatable.

var greenSpeed: Float

The speed, in seconds, at which the green color component changes over the lifetime of the cell. Animatable.

var blueSpeed: Float

The speed, in seconds, at which the blue color component changes over the lifetime of the cell. Animatable.

var alphaSpeed: Float

The speed, in seconds, at which the alpha component changes over the lifetime of the cell. Animatable.

var magnificationFilter: String

The filter used when increasing the size of the content.

var minificationFilter: String

The filter used when reducing the size of the content.

var minificationFilterBias: Float

The bias factor used by the minification filter to determine the levels of detail.

var scale: CGFloat

Specifies the scale factor applied to the cell. Animatable.

var scaleRange: CGFloat

Specifies the range over which the scale value can vary. Animatable.

var contentsScale: CGFloat

The scale factor of the cell contents.

var name: String?

The name of the cell.

var style: [AnyHashable : Any]?

An optional dictionary containing additional style values that are not explicitly defined by the receiver.

### Setting Emitter Cell Motion Attributes

var spin: CGFloat

The rotational velocity, measured in radians per second, to apply to the cell. Animatable.

var spinRange: CGFloat

The amount by which the spin of the cell can vary over its lifetime. Animatable.

var emissionLatitude: CGFloat

The latitudinal orientation of the emission angle. Animatable.

var emissionLongitude: CGFloat

The longitudinal orientation of the emission angle. Animatable.

var emissionRange: CGFloat

The angle, in radians, defining a cone around the emission angle. Animatable.

### Setting Emitter Cell Temporal Attributes

var lifetime: Float

The lifetime of the cell, in seconds. Animatable.

var lifetimeRange: Float

The mean value by which the lifetime of the cell can vary. Animatable.

var birthRate: Float

The number of emitted objects created every second. Animatable.

var scaleSpeed: CGFloat

The speed at which the scale changes over the lifetime of the cell. Animatable.

var velocity: CGFloat

The initial velocity of the cell. Animatable.

var velocityRange: CGFloat

The amount by which the velocity of the cell can vary. Animatable.

var xAcceleration: CGFloat

The x component of an acceleration vector applied to cell.

var yAcceleration: CGFloat

The y component of an acceleration vector applied to cell.

var zAcceleration: CGFloat

The z component of an acceleration vector applied to cell.

### Using Key-Value Coding Extensions

class func defaultValue(forKey: String) -> Any?

Returns the default value of the property with the specified key.

func shouldArchiveValue(forKey: String) -> Bool

Returns a Boolean value indicating whether the value for a given key should be archived.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Particle Systems

class CAEmitterLayer

A layer that emits, animates, and renders a particle system.

