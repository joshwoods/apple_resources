

- Model I/O
-  MDLMaterialPropertyType 

Enumeration

# MDLMaterialPropertyType

Options for the data type of a material property, used by the type property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLMaterialPropertyType
```

## Overview

Reading a material property’s value using an accessor for a type other than that corresponding to the type property produces undefined results.

## Topics

### Constants

case none

The material property’s value has not been initialized.

case string

The material’s value is a string.

case URL

The material property’s value is a URL—typically, a URL referencing a texture image.

case texture

The material property’s value is a MDLTextureSampler object that provides both a texture image and texture rendering parameters.

case color

The material property’s value is a uniform color.

case float

The material property’s value is a floating-point scalar.

case float2

The material property’s value is a 2-component floating-point vector.

case float3

The material property’s value is a 3-component floating-point vector.

case float4

The material property’s value is a 4-component floating-point vector.

case matrix44

The material property’s value is a 4 x 4 floating-point matrix.

### Enumeration Cases

case buffer

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum MDLMaterialSemantic

Options for the semantic use of a material property’s value in rendering a particular surface appearance; used by the semantic property.

