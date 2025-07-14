

- Swift
-  KeyPath 

Class

# KeyPath

A key path from a specific root type to a specific resulting value type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class KeyPath
```

## Overview

The most common way to make an instance of this type is by using a key-path expression like `\SomeClass.someProperty`. For more information, see Key-Path Expressions in *The Swift Programming Language*.

## Relationships

### Inherits From

- PartialKeyPath

### Inherited By

- WritableKeyPath

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Hashable

## See Also

### Key Paths

class PartialKeyPath

A partially type-erased key path, from a concrete root type to any resulting value type.

class AnyKeyPath

A type-erased key path, from any root type to any resulting value type.

