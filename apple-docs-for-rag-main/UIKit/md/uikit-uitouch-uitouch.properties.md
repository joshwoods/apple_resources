

- UIKit
- UITouch
-  UITouch.Properties 

Structure

# UITouch.Properties

A bit mask of touch properties that may get updated.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
struct Properties
```

## Topics

### Constants

static var force: UITouch.Properties

A touch property, representing force, in a bit mask.

static var azimuth: UITouch.Properties

A touch property, representing azimuth, in a bit mask.

static var altitude: UITouch.Properties

A touch property, representing altitude, in a bit mask.

static var location: UITouch.Properties

A touch property, representing location, in a bit mask.

static var roll: UITouch.Properties

A touch property, representing barrel-roll angle, in a bit mask.

### Initializers

init(rawValue: Int)

Creates a structure that represents the properties of a touch object.

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

### Managing estimated touch attributes

var estimatedProperties: UITouch.Properties

A set of touch properties whose values contain only estimates.

var estimatedPropertiesExpectingUpdates: UITouch.Properties

The set of touch properties for which updated values are expected in the future.

var estimationUpdateIndex: NSNumber?

An index number that lets you correlate an updated touch with the original touch.

