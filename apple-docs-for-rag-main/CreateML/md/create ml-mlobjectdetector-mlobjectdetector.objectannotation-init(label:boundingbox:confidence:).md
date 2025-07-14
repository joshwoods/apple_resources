

- Create ML
- MLObjectDetector
- MLObjectDetector.ObjectAnnotation
-  init(label:boundingBox:confidence:) 

Initializer

# init(label:boundingBox:confidence:)

Creates an annotation for an item an object detector finds in an image.

macOS 10.15+

``` source
init(
    label: String,
    boundingBox: CGRect,
    confidence: Double
)
```

## Parameters 

`label`  

The name of the item.

`boundingBox`  

The location of the item in an image.

`confidence`  

The confidence score of the item in the image. The value must be in the range `[0.0, 1.0]`, where `1.0` is the most confident.

## Discussion

You don’t use this initializer to create an object annotation yourself. The object detector uses it to create object annotations when it makes predictions on your images, such as when you use prediction(from:).

