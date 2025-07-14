

- Contacts
- CNError
-  keyPaths 

Instance Property

# keyPaths

An array of key paths associated with the error.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var keyPaths: [String]? { get }
```

## Discussion

For validation errors, this contains key paths to specific object properties.

## See Also

### Error details

var affectedRecordIdentifiers: [String]?

An array of strings that uniquely identify the records affected by the error.

var affectedRecords: [AnyObject]?

An array of record objects for which the error applies.

enum Code

Error codes that the system may return when you use Contacts framework methods.

