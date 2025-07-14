

- Core ML
- MLModelCollection
-  MLModelCollection.Entry Deprecated

Class

# MLModelCollection.Entry

A model and its identifier within a model collection.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedvisionOS 1.0–1.1Deprecated

``` source
class Entry
```

Deprecated

Use Background Assets or URLSession instead.

## Topics

### Identifying a Model

var modelIdentifier: String

The name of the model, which is unique to the collection.

### Locating a Compiled Model File

var modelURL: URL

The compiled model’s location on the device’s file system.

### Comparing Model Collection Entries

func isEqual(to: MLModelCollection.Entry) -> Bool

Returns a Boolean value that indicates whether the two entries are equal.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Retreiving Models from a Collection

var entries: [String : MLModelCollection.Entry]

A dictionary of model entries keyed to the models’ identifiers.

Deprecated

