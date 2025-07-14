

- Game Controller
-  GCPhysicalInputElement 

Protocol

# GCPhysicalInputElement

The common properties of physical input elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCPhysicalInputElement : NSObjectProtocol
```

## Topics

### Getting a localized name

var localizedName: String?

The localized name for the element.

**Required**

### Displaying a symbol

var sfSymbolsName: String?

A system symbol for the element.

**Required**

### Accessing elements by key

var aliases: Set&lt;String>

The element’s aliases to use when accessing it with the subscript notation.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- GCAxisElement
- GCButtonElement
- GCDirectionPadElement
- GCSwitchElement

### Conforming Types

- GCGearShifterElement
- GCSteeringWheelElement

## See Also

### Elements

struct GCPhysicalInputElementCollection

A collection of physical input elements.

protocol GCButtonElement

The common properties of an element that represents a momentary switch, such as a push button.

protocol GCAxisElement

The common properties for an element that represents an absolute or relative input value along an axis.

protocol GCSwitchElement

The common properties for an element that represents a switch.

protocol GCDirectionPadElement

The common properties of elements that represent directional pads.

