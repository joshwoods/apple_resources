

- Create ML Components
- Pose
-  boundingBoxArea(confidenceThreshold:) 

Instance Method

# boundingBoxArea(confidenceThreshold:)

Computes the bounding box area of the pose.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func boundingBoxArea(confidenceThreshold: Float = 0.2) -> Float
```

## Parameters 

`confidenceThreshold`  

A threshold confidence between 0 to 1 for the keypoints to be considered valid to compute the bounding box area. The default value is 0.2.

