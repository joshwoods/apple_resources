

- Create ML Components
- JointPoint
-  init(\_:location:confidence:) 

Initializer

# init(\_:location:confidence:)

Creates a joint point with its key, location and confidence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    _ key: JointKey,
    location: CGPoint,
    confidence: Float
)
```

## Parameters 

`key`  

Joint point identifier name.

`location`  

A point indicating the location of the joint.

`confidence`  

The detection confidence for the joint.

