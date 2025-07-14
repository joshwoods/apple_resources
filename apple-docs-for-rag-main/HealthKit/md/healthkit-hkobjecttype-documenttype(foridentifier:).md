

- HealthKit
- HKObjectType
-  documentType(forIdentifier:) 

Type Method

# documentType(forIdentifier:)

Returns the shared document type for the provided identifier.

iOS 10.0–18.4DeprecatediPadOS 10.0–18.4DeprecatedMac Catalyst 13.1+macOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 3.0–11.4Deprecated

``` source
class func documentType(forIdentifier identifier: HKDocumentTypeIdentifier) -> HKDocumentType?
```

## Parameters 

`identifier`  

A document type identifier. For a list of valid identifiers, see HKDocumentTypeIdentifier.

## Return Value

The shared HKDocumentType instance based on the provided identifier.

## Discussion

This method returns an instance of the HKQuantityType concrete subclass. HealthKit uses document types to manage medical documents. Use document type instances to create document samples that you can save in the HealthKit store. For more information, see HKDocumentSample.

## See Also

### Creating document types

struct HKDocumentTypeIdentifier

The identifiers for documents.

