

- HealthKit
- HKCDADocumentSample
-  document 

Instance Property

# document

The CDA document.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
var document: HKCDADocument? { get }
```

## Discussion

If the user is authorized to access the document’s data, this property contains an HKCDADocument object representing that data. Otherwise, it is set to `nil`.

The user is asked to authorize each CDA document the first time that document is returned by an HKDocumentQuery query. The user can change the access permissions in the Health app.

For samples returned by an HKSampleQuery or an HKAnchoredObjectQuery, this property is always set to `nil`. To access the document’s data from these samples, create a HKDocumentQuery query for the sample’s UUID.

## See Also

### Accessing the Document

class HKCDADocument

An object representing a Clinical Document Architecture (CDA) document in HealthKit.

