

- ARKit
- ARFaceGeometry
-  init(blendShapes:) 

Initializer

# init(blendShapes:)

Creates a face geometry matching the facial expression described in the specified dictionary.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
init?(blendShapes: [ARFaceAnchor.BlendShapeLocation : NSNumber])
```

## Parameters 

`blendShapes`  

A dictionary of blend shape coefficients describing a facial expression in terms of the positions of specific facial features. For any coefficient not specified in this dictionary, ARKit assumes a value of `0.0`.

## Return Value

A face geometry object, or `nil` if ARKit face tracking is not supported on the current device.

## Discussion

Each key in the `blendShapes` dictionary is an ARFaceAnchor.BlendShapeLocation constant identifying a facial feature. The corresponding value is the position of that feature relative to its neutral configuration, ranging from `0.0` (neutral) to `1.0` (maximum movement).

The format of this dictionary is identical to that provided by the ARFaceAnchor blendShapes property. You can use that property and this initializer to efficiently save and restore facial expression data; the serialized form of a blend shapes dictionary is more portable than that of the face mesh those coefficients describe.

