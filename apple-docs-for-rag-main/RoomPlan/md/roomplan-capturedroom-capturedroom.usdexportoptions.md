

- RoomPlan
- CapturedRoom
-  CapturedRoom.USDExportOptions 

Structure

# CapturedRoom.USDExportOptions

Options that determine the underlying data format of a scan export.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct USDExportOptions
```

## Overview

The `exportOptions` parameter of the captured room (CapturedRoom) and captured structure (CapturedStructure) functions `export(to:metadataURL:modelProvider:exportOptions:)` are of this type.

The following table lists the features that each export option supports in the output result.

| Feature per export option | Parametric | Mesh | Model |
|----|----|----|----|
| Changing the size or position of objects, windows, or doors | ✔ |  |  |
| Boolean operations | ✔ |  |  |
| Section positions and labels | ✔ | ✔ | ✔ |
| Polygonal walls |  | ✔ | ✔ |
| Windows, doors, and other openings cut out of wall geometry |  | ✔ | ✔ |
| The recessed areas of a sink or fireplace |  | ✔ | ✔ |
| ModelProvider models |  |  | ✔ |

## Topics

### Choosing an export option

static let parametric: CapturedRoom.USDExportOptions

An export option that formats the output file as a collection of size-dependent primitives.

static let mesh: CapturedRoom.USDExportOptions

An export option that formats the output file as a collection of size-independant triangles that connect to form a mesh.

static let model: CapturedRoom.USDExportOptions

An export option that formats the output file as a collection of 3D models.

### Creating an export option

init(rawValue: Int32)

Creates an export option with the specified raw value.

let rawValue: Int32

A raw value for the export option.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### 3D Asset Output

Providing custom models for captured rooms and structure exports

Enhance the look of an exported 3D model by substituting object bounding boxes with detailed 3D renditions.

class RoomBuilder

An object that generates a 3D asset from room-capture data.

class StructureBuilder

An object that combines multiple scan sessions into a single captured result.

