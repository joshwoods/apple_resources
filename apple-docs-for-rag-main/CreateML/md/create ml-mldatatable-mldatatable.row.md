

- Create ML
- MLDataTable
-  MLDataTable.Row 

Structure

# MLDataTable.Row

A row of untyped values in a data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct Row
```

## Topics

### Accessing parameters

var keys: MLDataTable.Row.Keys

var values: MLDataTable.Row.Values

typealias Key

typealias Keys

typealias Value

struct Values

### Getting a row

func index(forKey: MLDataTable.Row.Key) -> MLDataTable.Row.Index?

### Accessing rows

subscript(MLDataTable.Row.Key) -> MLDataTable.Row.Value?

subscript&lt;T>(MLDataTable.Row.Key, T.Type) -> T?

### Default Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible
- Equatable
- Sequence

## See Also

### Supporting types

typealias Element

The Element of a DataTable is a Row. This is represented as a Dictionary-like type containing all Column names and their corresponding values.

