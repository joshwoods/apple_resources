

- ARKit
-  ARObjectAnchor 

Class

# ARObjectAnchor

An anchor for a real-world 3D object that ARKit detects in the physical environment.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class ARObjectAnchor
```

## Overview

When you run a world-tracking AR session and specify ARReferenceObject objects for the session configuration’s detectionObjects property, ARKit searches for those objects in the real-world environment. When the session recognizes an object, it automatically adds to its list of anchors an ARObjectAnchor for each detected object.

To place virtual 3D content that matches the position or size of the detected object, use the anchor’s inherited transform property together with the center and extent of the anchor’s referenceObject.

## Topics

### Identifying Detected Objects

var referenceObject: ARReferenceObject

The detected object referenced by the object anchor.

## Relationships

### Inherits From

- ARAnchor

### Conforms To

- ARAnchorCopying
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Physical Objects

Visualizing and interacting with a reconstructed scene

Estimate the shape of the physical environment using a polygonal mesh.

Scanning and Detecting 3D Objects

Record spatial features of real-world objects, then use the results to find those objects in the user’s environment and trigger AR content.

class ARReferenceObject

The description of a 3D object that you want ARKit to detect in the physical environment.

