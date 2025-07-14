

- Game Controller
-  GCAxisElement 

Protocol

# GCAxisElement

The common properties for an element that represents an absolute or relative input value along an axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCAxisElement : GCPhysicalInputElement
```

## Topics

### Getting the inputs

var absoluteInput: (any GCAxisInput)?

An input object that provides absolute axis values.

**Required**

var relativeInput: any GCRelativeInput

An input object that provides relative axis values.

**Required**

## Relationships

### Inherits From

- GCPhysicalInputElement
- NSObjectProtocol

### Conforming Types

- GCSteeringWheelElement

## See Also

### Elements

struct GCPhysicalInputElementCollection

A collection of physical input elements.

protocol GCPhysicalInputElement

The common properties of physical input elements.

protocol GCButtonElement

The common properties of an element that represents a momentary switch, such as a push button.

protocol GCSwitchElement

The common properties for an element that represents a switch.

protocol GCDirectionPadElement

The common properties of elements that represent directional pads.

