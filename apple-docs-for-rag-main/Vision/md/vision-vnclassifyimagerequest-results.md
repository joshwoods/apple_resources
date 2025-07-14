

- Vision
- VNClassifyImageRequest
-  results 

Instance Property

# results

The results of the image classification request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var results: [VNClassificationObservation]? { get }
```

## See Also

### Accessing Results

func supportedIdentifiers() throws -> [String]

Returns the classification identifiers that the request supports in its current configuration.

class VNClassificationObservation

An object that represents classification information that an image-analysis request produces.

class func knownClassifications(forRevision: Int) throws -> [VNClassificationObservation]

Requests the collection of classifications that the Vision framework recognizes.

Deprecated

