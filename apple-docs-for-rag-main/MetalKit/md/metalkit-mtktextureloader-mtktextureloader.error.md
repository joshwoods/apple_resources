

- MetalKit
- MTKTextureLoader
-  MTKTextureLoader.Error 

Structure

# MTKTextureLoader.Error

Errors returned by the texture loader.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct Error
```

## Topics

### Initializers

init(rawValue: String)

### Keys

static let domain: MTKTextureLoader.Error

The error domain used by `MetalKit` when returning texture loading errors.

static let key: MTKTextureLoader.Error

The key used to retrieve an error string from an error object’s userInfo dictionary.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

