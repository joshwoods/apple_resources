

- ARKit
- ARObjectAnchor
-  referenceObject 

Instance Property

# referenceObject

The detected object referenced by the object anchor.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var referenceObject: ARReferenceObject { get }
```

## Discussion

This object is always one of the ARReferenceObject objects you provided in the detectionObjects array when configuring the session.

