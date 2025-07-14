

- Create ML
- MLDataValue
-  MLDataValue.DictionaryType 

Structure

# MLDataValue.DictionaryType

A dictionary of named data values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct DictionaryType
```

## Topics

### Creating a dictionary type

init([MLDataValue : MLDataValue])

init&lt;S>(uniqueKeysWithValues: S)

typealias Key

typealias Value

### Getting an element

subscript(MLDataValue.DictionaryType.Key) -> MLDataValue.DictionaryType.Value?

### Default Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

MLDataValueConvertible Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- MLDataValueConvertible
- Sequence

## See Also

### Accessing dictionary values

var dictionaryValue: MLDataValue.DictionaryType?

The underlying dictionary.

