

- Contacts
- CNError
-  affectedRecordIdentifiers 

Instance Property

# affectedRecordIdentifiers

An array of strings that uniquely identify the records affected by the error.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var affectedRecordIdentifiers: [String]? { get }
```

## See Also

### Error details

var affectedRecords: [AnyObject]?

An array of record objects for which the error applies.

enum Code

Error codes that the system may return when you use Contacts framework methods.

var keyPaths: [String]?

An array of key paths associated with the error.

