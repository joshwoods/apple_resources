

- GLKit
-  GLKFogMode 

Enumeration

# GLKFogMode

A mode that describes how the fog component is calculated for the fragment.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
enum GLKFogMode
```

## Topics

### Constants

case exp

The fog component is calculated as `exp(-density * distance)` and clamped to the range `[0.0, 1.0]`.

case exp2

The fog component is calculated as `exp(-(density * distance)^2)` and clamped to the range `[0.0, 1.0]`.

case linear

The fog component is calculated as `(end - distance) / (end - start)` and clamped to the range `[0.0, 1.0]`.

### Initializers

init?(rawValue: GLint)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

