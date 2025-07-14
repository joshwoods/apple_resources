

- MetalKit
-  MTKModelError 

Structure

# MTKModelError

Constants used to declare Model Errors.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct MTKModelError
```

## Topics

### Initializing a Raw Constant

init(rawValue: String)

### Finding Model Error Constants

static let domain: MTKModelError

The error domain used by MetalKit when returning mesh initialization errors.

static let key: MTKModelError

The key used to retrieve an error string from an error object’s userInfo dictionary.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

