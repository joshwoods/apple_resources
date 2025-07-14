

- GLKit
-  GLKTextureEnvMode 

Enumeration

# GLKTextureEnvMode

The mode used to combine the texture with other color components.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
enum GLKTextureEnvMode
```

## Topics

### Constants

case replace

The output color is set to the color fetched from the texture. The input color is ignored.

case modulate

The output color is calculated by multiplying the texture’s color by the input color.

case decal

The output color is calculated by using the texture’s alpha component to blend the texture’s color with the input color.

### Initializers

init?(rawValue: GLint)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum GLKTextureTarget

The kind of texture pointed to by the property.

