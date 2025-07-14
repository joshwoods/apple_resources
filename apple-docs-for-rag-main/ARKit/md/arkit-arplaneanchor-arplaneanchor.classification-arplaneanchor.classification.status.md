

- ARKit
- ARPlaneAnchor
- ARPlaneAnchor.Classification
-  ARPlaneAnchor.Classification.Status 

Enumeration

# ARPlaneAnchor.Classification.Status

Reasons ARKit is unable to classify a plane.

iOS 12.0+iPadOS 12.0+

``` source
enum Status
```

## Overview

ARPlaneAnchor.Classification.Status tells you why a plane anchor’s classification is ARPlaneAnchor.Classification.none(_:).

## Topics

### Classification Status

case notAvailable

ARKit cannot currently provide plane classification information.

case undetermined

ARKit has not yet produced a classification for the plane anchor.

case unknown

ARKit has completed its classification process for the plane anchor, but the result is inconclusive.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Missing Classification Status

case none(ARPlaneAnchor.Classification.Status)

No classification is available for the plane anchor.

