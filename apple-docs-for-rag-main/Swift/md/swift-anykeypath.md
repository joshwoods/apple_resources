

- Swift
-  AnyKeyPath 

Class

# AnyKeyPath

A type-erased key path, from any root type to any resulting value type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AnyKeyPath
```

## Topics

### Type Properties

static var rootType: any Any.Type

The root type for this key path.

static var valueType: any Any.Type

The value type for this key path.

### Default Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Inherited By

- PartialKeyPath

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable

## See Also

### Key Paths

class KeyPath

A key path from a specific root type to a specific resulting value type.

class PartialKeyPath

A partially type-erased key path, from a concrete root type to any resulting value type.

