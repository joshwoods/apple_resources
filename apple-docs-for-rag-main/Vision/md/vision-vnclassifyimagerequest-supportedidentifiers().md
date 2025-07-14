

- Vision
- VNClassifyImageRequest
-  supportedIdentifiers() 

Instance Method

# supportedIdentifiers()

Returns the classification identifiers that the request supports in its current configuration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func supportedIdentifiers() throws -> [String]
```

## Return Value

An array of supported identifiers.

## See Also

### Accessing Results

var results: [VNClassificationObservation]?

The results of the image classification request.

class VNClassificationObservation

An object that represents classification information that an image-analysis request produces.

class func knownClassifications(forRevision: Int) throws -> [VNClassificationObservation]

Requests the collection of classifications that the Vision framework recognizes.

Deprecated

