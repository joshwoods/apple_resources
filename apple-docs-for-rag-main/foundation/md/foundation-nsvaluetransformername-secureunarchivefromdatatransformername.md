

- Foundation
- NSValueTransformerName
-  secureUnarchiveFromDataTransformerName 

Type Property

# secureUnarchiveFromDataTransformerName

The name of the value transformer that creates then returns an object by attempting to unarchive the data to a class that supports secure coding.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static let secureUnarchiveFromDataTransformerName: NSValueTransformerName
```

## Discussion

The transformer this property references returns the NSData instance created by archiving the value using secure keyed archiving. This transformer requires that an object implement the NSSecureCoding protocol in order to archive and unarchive with this transformer.

## See Also

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

