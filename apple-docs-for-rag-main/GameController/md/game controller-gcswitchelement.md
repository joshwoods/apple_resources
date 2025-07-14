

- Game Controller
-  GCSwitchElement 

Protocol

# GCSwitchElement

The common properties for an element that represents a switch.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCSwitchElement : GCPhysicalInputElement
```

## Topics

### Getting input state

var positionInput: any GCSwitchPositionInput

The input object that provides the position of the switch.

**Required**

## Relationships

### Inherits From

- GCPhysicalInputElement
- NSObjectProtocol

## See Also

### Elements

struct GCPhysicalInputElementCollection

A collection of physical input elements.

protocol GCPhysicalInputElement

The common properties of physical input elements.

protocol GCButtonElement

The common properties of an element that represents a momentary switch, such as a push button.

protocol GCAxisElement

The common properties for an element that represents an absolute or relative input value along an axis.

protocol GCDirectionPadElement

The common properties of elements that represent directional pads.

