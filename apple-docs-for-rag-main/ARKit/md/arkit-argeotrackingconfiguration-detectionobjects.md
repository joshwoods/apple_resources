

- ARKit
- ARGeoTrackingConfiguration
-  detectionObjects 

Instance Property

# detectionObjects

A set of 3D objects that the framework attempts to detect in the user’s environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var detectionObjects: Set { get set }
```

## Discussion

Use this property to choose known 3D objects for ARKit to find in the user’s environment and present as ARObjectAnchor for use in your AR experience.

To create reference objects for detection, scan them in a world-tracking session and use ARWorldMap to extract ARReferenceObject instances. You can then save reference objects as files and package them in any ARKit app you create using an Xcode asset catalog.

