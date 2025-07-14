

- Game Controller
-  GCPhysicalInputElementTypedName 

Protocol

# GCPhysicalInputElementTypedName

A type-safe name for accessing elements of a physical input element collection.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS

``` source
protocol GCPhysicalInputElementTypedName : Hashable, RawRepresentable, Sendable where Self.RawValue == String
```

## Topics

### Associated type

associatedtype PhysicalInputElement : GCPhysicalInputElement

A placeholder for the type that adopts this protocol.

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable
- RawRepresentable
- Sendable

### Conforming Types

- GCAxisElementName
- GCButtonElementName
- GCDirectionPadElementName
- GCPhysicalInputElementName
- GCSwitchElementName

## See Also

### Element names

struct GCPhysicalInputElementName

The name of a physical input element.

struct GCButtonElementName

The names of the button elements.

struct GCAxisElementName

The names for the elements that provide values along an axis.

struct GCSwitchElementName

The name for an element that represents a switch.

struct GCDirectionPadElementName

The names for directional pad elements.

Extended gamepad input names

Constants for names of extended gamepad elements.

DualShock controller input names

Constants for names of DualShock 4 elements.

Xbox controller input names

Constants for names of Xbox elements.

Micro gamepad input names

Constants for names of micro gamepad elements.

Directional Gamepad Input Names

Constants for names of directional pad elements.

