

- Foundation
- NSValueTransformerName
-  isNotNilTransformerName 

Type Property

# isNotNilTransformerName

This value transformer returns true if the value is non-`nil`.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let isNotNilTransformerName: NSValueTransformerName
```

## Discussion

This transformer is not reversible.

## See Also

### Type Properties

static let isNilTransformerName: NSValueTransformerName

This value transformer returns true if the value is `nil`.

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

