

- Vision
- DetectFaceCaptureQualityRequest
-  DetectFaceCaptureQualityRequest.Revision 

Enumeration

# DetectFaceCaptureQualityRequest.Revision

A type that describes the algorithm or implementation that the request performs.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum Revision
```

## Topics

### Getting the revision

case revision3

An algorithm or implementation that represents the third revision.

## Relationships

### Conforms To

- Comparable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the revision

let revision: DetectFaceCaptureQualityRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectFaceCaptureQualityRequest.Revision]

The collection of revisions the request supports.

