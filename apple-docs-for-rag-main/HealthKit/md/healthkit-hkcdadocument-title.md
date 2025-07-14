

- HealthKit
- HKCDADocument
-  title 

Instance Property

# title

The document’s title.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
var title: String { get }
```

## Discussion

HealthKit automatically extracts the document’s title from the CDA’s XML data.

## See Also

### Accessing the Document’s Data

var authorName: String

The document’s author.

var custodianName: String

The name of the organization responsible for the document.

var documentData: Data?

The CDA document stored as XML data.

var patientName: String

The patient’s name.

