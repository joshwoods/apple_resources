

- HealthKit
- HKCDADocument
-  custodianName 

Instance Property

# custodianName

The name of the organization responsible for the document.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
var custodianName: String { get }
```

## Discussion

Usually, this is the treating institution’s name.

HealthKit automatically extracts the custodian’s name from the CDA’s XML data.

## See Also

### Accessing the Document’s Data

var authorName: String

The document’s author.

var documentData: Data?

The CDA document stored as XML data.

var patientName: String

The patient’s name.

var title: String

The document’s title.

