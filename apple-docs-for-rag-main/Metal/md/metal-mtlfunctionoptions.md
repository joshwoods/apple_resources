

- Metal
-  MTLFunctionOptions 

Structure

# MTLFunctionOptions

Options that define how Metal creates the function object.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct MTLFunctionOptions
```

## Topics

### Creating Function Options

init(rawValue: UInt)

Creates a new function options structure from a raw value.

### Function Option Values

static var compileToBinary: MTLFunctionOptions

An option that tells Metal to compile the function to a binary format for dynamic linking.

### Type Properties

static var failOnBinaryArchiveMiss: MTLFunctionOptions

static var storeFunctionInMetalPipelinesScript: MTLFunctionOptions

static var storeFunctionInMetalScript: MTLFunctionOptionsDeprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Identifying Shader Functions

var device: any MTLDevice

The device object that created the shader function.

**Required**

var label: String?

A string that identifies the shader function.

**Required**

var functionType: MTLFunctionType

The shader function’s type.

**Required**

var name: String

The function’s name.

**Required**

enum MTLFunctionType

The type of a top-level Metal Shading Language (MSL) function.

var options: MTLFunctionOptions

The options that Metal used to compile this function.

**Required**

