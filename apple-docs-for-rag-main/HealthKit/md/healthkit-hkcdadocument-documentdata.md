

- HealthKit
- HKCDADocument
-  documentData 

Instance Property

# documentData

The CDA document stored as XML data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
var documentData: Data? { get }
```

## Discussion

The CDA document’s XML format is specified by the Clinical Document Architecture, R2 standard. .

When using an HKDocumentQuery object to retrieve documents from the HealthKit store, if the query’s includeDocumentData property is set to false, the retrieved documents will have `nil`-valued `documentData` properties.

## See Also

### Accessing the Document’s Data

var authorName: String

The document’s author.

var custodianName: String

The name of the organization responsible for the document.

var patientName: String

The patient’s name.

var title: String

The document’s title.

