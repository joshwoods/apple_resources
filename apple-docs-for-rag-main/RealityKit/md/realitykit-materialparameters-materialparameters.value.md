

- RealityKit
- MaterialParameters
-  MaterialParameters.Value 

Enumeration

# MaterialParameters.Value

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum Value
```

## Topics

### Enumeration Cases

case bool(Bool)

case color(CGColor)

case float(Float)

case float2x2(float2x2)

case float3x3(float3x3)

case float4x4(float4x4)

case int(Int32)

case simd2Float(SIMD2&lt;Float>)

case simd3Float(SIMD3&lt;Float>)

case simd4Float(SIMD4&lt;Float>)

case texture(MaterialParameters.Texture)

case textureResource(TextureResource)

### Instance Properties

var colorValue: NSColor?

var colorValue: UIColor?

### Type Methods

static func color(NSColor) -> MaterialParameters.Value

static func color(UIColor) -> MaterialParameters.Value

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable

