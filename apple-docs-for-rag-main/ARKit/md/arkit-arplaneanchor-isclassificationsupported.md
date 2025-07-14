

- ARKit
- ARPlaneAnchor
-  isClassificationSupported 

Type Property

# isClassificationSupported

A Boolean value that indicates whether plane classification is available on the current device.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class var isClassificationSupported: Bool { get }
```

## Discussion

Plane classification is available on iOS devices with A12 or later GPU.

On devices without plane classification support, all plane anchors report a classification value of ARPlaneClassificationNone and a classificationStatus value of ARPlaneClassificationStatusNotAvailable.

## See Also

### Classifying a Plane

var classification: ARPlaneAnchor.Classification

A general characterization of what kind of real-world surface the plane anchor represents.

enum Classification

Possible characterizations of real-world surfaces represented by plane anchors.

