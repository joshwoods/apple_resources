

- Game Controller
-  GCDirectionPadElement 

Protocol

# GCDirectionPadElement

The common properties of elements that represent directional pads.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCDirectionPadElement : GCPhysicalInputElement
```

## Topics

### Directional buttons

var left: any GCLinearInput &amp; GCPressedStateInput

The input object that represents the left button on the directional pad.

**Required**

var right: any GCLinearInput &amp; GCPressedStateInput

The input object that represents the right button on the directional pad.

**Required**

var up: any GCLinearInput &amp; GCPressedStateInput

The input object that represents the up button on the directional pad.

**Required**

var down: any GCLinearInput &amp; GCPressedStateInput

The input object that represents the down button on the directional pad.

**Required**

### Axes

var xAxis: any GCAxisInput

The input object that represents the x-axis on the directional pad.

**Required**

var yAxis: any GCAxisInput

The input object that represents the y-axis on the directional pad.

**Required**

var xyAxes: any GCAxis2DInput

The location of the directional pad represented as a point.

**Required**

protocol GCAxis2DInput

The common properties of inputs that provide a normalized point in a two-dimensional coordinate system with a fixed origin.

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

protocol GCSwitchElement

The common properties for an element that represents a switch.

