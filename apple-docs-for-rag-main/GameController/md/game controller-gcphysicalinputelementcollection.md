

- Game Controller
-  GCPhysicalInputElementCollection 

Structure

# GCPhysicalInputElementCollection

A collection of physical input elements.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS

``` source
struct GCPhysicalInputElementCollection where T : GCPhysicalInputElement
```

## Topics

### Accessing elements by name

subscript(GCDirectionPadElementName) -> T?

Accesses a contiguous subrange of a collection of direction pad elements.

subscript(GCAxisElementName) -> T?

Accesses a contiguous subrange of a collection of axis elements.

subscript(GCButtonElementName) -> T?

Accesses a contiguous subrange of a collection of button elements.

subscript(GCSwitchElementName) -> T?

Accesses a contiguous subrange of a collection of switch elements.

subscript(GCPhysicalInputElementName) -> T?

### Subscripts

subscript(String) -> T?

Accesses a contiguous subrange of the collection’s elements.

subscript&lt;Name>(Name) -> Name.PhysicalInputElement?

Accesses the collection’s elements using the element’s name.

subscript&lt;Name>(Name) -> (any GCPhysicalInputElement)?

Accesses the collection’s elements using the element’s name.

## Relationships

### Conforms To

- Collection
- Sequence

## See Also

### Elements

protocol GCPhysicalInputElement

The common properties of physical input elements.

protocol GCButtonElement

The common properties of an element that represents a momentary switch, such as a push button.

protocol GCAxisElement

The common properties for an element that represents an absolute or relative input value along an axis.

protocol GCSwitchElement

The common properties for an element that represents a switch.

protocol GCDirectionPadElement

The common properties of elements that represent directional pads.

