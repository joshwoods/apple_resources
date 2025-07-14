

- Foundation
-  NSValueTransformerName 

Structure

# NSValueTransformerName

Named value transformers defined by `NSValueTransformer`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSValueTransformerName
```

## Topics

### Type Properties

static let isNilTransformerName: NSValueTransformerName

This value transformer returns true if the value is `nil`.

static let isNotNilTransformerName: NSValueTransformerName

This value transformer returns true if the value is non-`nil`.

static let keyedUnarchiveFromDataTransformerName: NSValueTransformerName

The name of the value transformer that attempts to unarchive data stored inside a keyed archive in an object you provide.

Deprecated

static let negateBooleanTransformerName: NSValueTransformerName

This value transformer negates a boolean value, transforming true to false and false to true.

static let unarchiveFromDataTransformerName: NSValueTransformerName

The name of the value transformer that attempts to unarchive data from an object you provide.

Deprecated

static let secureUnarchiveFromDataTransformerName: NSValueTransformerName

The name of the value transformer that creates then returns an object by attempting to unarchive the data to a class that supports secure coding.

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Using the Name-Based Registry

class func setValueTransformer(ValueTransformer?, forName: NSValueTransformerName)

Registers the provided value transformer with a given identifier.

init?(forName: NSValueTransformerName)

Returns the value transformer identified by a given identifier.

class func valueTransformerNames() -> [NSValueTransformerName]

Returns an array of all the registered value transformers.

