

- Model I/O
-  MDLIndexBitDepth 

Enumeration

# MDLIndexBitDepth

Options for the size of integer data in a submesh’s index buffer, used by the indexType property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLIndexBitDepth
```

## Overview

For optimum performance, an index buffer should generally use the smallest data type that fits the number of indices it contains.

## Topics

### Constants

case invalid

The submesh has not been initialized or its data type is unknown.

case uInt8

Each index in the submesh’s index buffer is an 8-bit integer.

case uInt16

Each index in the submesh’s index buffer is a 16-bit integer.

case uInt32

Each index in the submesh’s index buffer is a 32-bit integer.

### Initializers

init?(rawValue: UInt)

### Type Properties

static var uint16: MDLIndexBitDepth

static var uint32: MDLIndexBitDepth

static var uint8: MDLIndexBitDepth

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum MDLGeometryType

Types of geometric primitives for rendering a submesh, used by the geometryType property.

