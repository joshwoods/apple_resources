

- HealthKit
- HKCDADocument
-  authorName 

Instance Property

# authorName

The document’s author.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
var authorName: String { get }
```

## Discussion

Usually, this is the treating physician’s name.

HealthKit automatically extracts the author’s name from the CDA’s XML data.

## See Also

### Accessing the Document’s Data

var custodianName: String

The name of the organization responsible for the document.

var documentData: Data?

The CDA document stored as XML data.

var patientName: String

The patient’s name.

var title: String

The document’s title.

