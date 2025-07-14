

- ARKit
- ARPlaneAnchor
-  classification 

Instance Property

# classification

A general characterization of what kind of real-world surface the plane anchor represents.

iOS 12.0+iPadOS 12.0+

``` source
var classification: ARPlaneAnchor.Classification { get }
```

## Discussion

On supported devices, ARKit automatically attempts to characterize each detected plane, describing it as a real-world surface such as as a wall, floor, or table. You can then use this information to enhance the realism of your AR experience; for example, by placing certain virtual content only on floors.

Plane classification can take longer than plane detection, and ARKit reports classifications only for planes where it has a high confidence in the result. If ARKit currently has no classification result for a plane, this property’s value is ARPlaneAnchor.Classification.none(_:), with an associated ARPlaneAnchor.Classification.Status value indicating why.

Plane classification is available only on iPhone XS, iPhone XS Max, and iPhone XR. Before using classification results, check the isClassificationSupported class property to make sure you’re on a supported device.

## See Also

### Classifying a Plane

class var isClassificationSupported: Bool

A Boolean value that indicates whether plane classification is available on the current device.

enum Classification

Possible characterizations of real-world surfaces represented by plane anchors.

