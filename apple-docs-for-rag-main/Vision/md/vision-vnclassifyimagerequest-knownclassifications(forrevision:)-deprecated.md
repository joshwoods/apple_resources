

- Vision
- VNClassifyImageRequest
-  knownClassifications(forRevision:) Deprecated

Type Method

# knownClassifications(forRevision:)

Requests the collection of classifications that the Vision framework recognizes.

iOS 13.0–15.0DeprecatediPadOS 13.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.15–12.0DeprecatedtvOS 13.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func knownClassifications(forRevision requestRevision: Int) throws -> [VNClassificationObservation]
```

Deprecated

Use supportedIdentifiers() instead.

## Parameters 

`requestRevision`  

The revision of the request for which to report classifications.

## Return Value

An array of classifications for the revision, or `nil` if an error occurs.

## See Also

### Accessing Results

func supportedIdentifiers() throws -> [String]

Returns the classification identifiers that the request supports in its current configuration.

var results: [VNClassificationObservation]?

The results of the image classification request.

class VNClassificationObservation

An object that represents classification information that an image-analysis request produces.

