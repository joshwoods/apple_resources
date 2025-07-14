

- Vision
- GenerateImageFeaturePrintRequest
-  GenerateImageFeaturePrintRequest.Revision 

Enumeration

# GenerateImageFeaturePrintRequest.Revision

A type that describes the algorithm or implementation that the request performs.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum Revision
```

## Topics

### Getting the revision

case revision2

An algorithm or implementation that represents the second revision.

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

let revision: GenerateImageFeaturePrintRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [GenerateImageFeaturePrintRequest.Revision]

The collection of revisions the request supports.

