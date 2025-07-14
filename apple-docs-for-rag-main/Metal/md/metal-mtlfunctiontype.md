

- Metal
-  MTLFunctionType 

Enumeration

# MTLFunctionType

The type of a top-level Metal Shading Language (MSL) function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLFunctionType
```

## Topics

### Function Types

case vertex

A vertex function you can use in a render pipeline state object.

case fragment

A fragment function you can use in a render pipeline state object.

case kernel

A kernel you can use in a compute pipeline state object.

case intersection

A function you can use in an intersection function table.

case visible

A function you can use in a visible function table.

### Enumeration Cases

case mesh

case object

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

var options: MTLFunctionOptions

The options that Metal used to compile this function.

**Required**

struct MTLFunctionOptions

Options that define how Metal creates the function object.

