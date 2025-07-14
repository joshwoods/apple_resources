

- Game Controller
-  GCButtonElement 

Protocol

# GCButtonElement

The common properties of an element that represents a momentary switch, such as a push button.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCButtonElement : GCPhysicalInputElement
```

## Topics

### Getting input state

var touchedInput: (any GCTouchedStateInput)?

The input object that provides the touch state of the element.

**Required**

var pressedInput: any GCLinearInput &amp; GCPressedStateInput

The input object that provides the linear and press state of the element.

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

protocol GCAxisElement

The common properties for an element that represents an absolute or relative input value along an axis.

protocol GCSwitchElement

The common properties for an element that represents a switch.

protocol GCDirectionPadElement

The common properties of elements that represent directional pads.

