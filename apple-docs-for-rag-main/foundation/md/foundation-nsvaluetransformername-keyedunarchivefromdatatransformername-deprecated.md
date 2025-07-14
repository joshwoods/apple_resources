

- Foundation
- NSValueTransformerName
-  keyedUnarchiveFromDataTransformerName Deprecated

Type Property

# keyedUnarchiveFromDataTransformerName

The name of the value transformer that attempts to unarchive data stored inside a keyed archive in an object you provide.

iOS 3.0–12.0DeprecatediPadOS 3.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.3–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–5.0Deprecated

``` source
static let keyedUnarchiveFromDataTransformerName: NSValueTransformerName
```

Deprecated

Use secureUnarchiveFromDataTransformerName instead.

## Discussion

The transformer this property references returns the NSData instance created by archiving the value using keyed archiving. This transformer requires that an object implement the NSCoding protocol using keyed archiving in order to archive and unarchive with this transformer.

## See Also

### Type Properties

static let isNilTransformerName: NSValueTransformerName

This value transformer returns true if the value is `nil`.

static let isNotNilTransformerName: NSValueTransformerName

This value transformer returns true if the value is non-`nil`.

static let negateBooleanTransformerName: NSValueTransformerName

This value transformer negates a boolean value, transforming true to false and false to true.

static let unarchiveFromDataTransformerName: NSValueTransformerName

The name of the value transformer that attempts to unarchive data from an object you provide.

Deprecated

static let secureUnarchiveFromDataTransformerName: NSValueTransformerName

The name of the value transformer that creates then returns an object by attempting to unarchive the data to a class that supports secure coding.

