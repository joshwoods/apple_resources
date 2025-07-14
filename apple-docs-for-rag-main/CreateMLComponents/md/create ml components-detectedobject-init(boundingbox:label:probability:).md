

- Create ML Components
- DetectedObject
-  init(boundingBox:label:probability:) 

Initializer

# init(boundingBox:label:probability:)

Creates a detected object with bounding box, object label and confidence.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    boundingBox: CGRect,
    label: Label,
    probability: Float
)
```

## Parameters 

`boundingBox`  

The bounding box of the detected object.

`label`  

The label of the detected object.

`probability`  

The detection confidence. The value will always be between 0.0 and 1.0

