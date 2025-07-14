

- Vision
- VNSaliencyImageObservation
-  salientObjects 

Instance Property

# salientObjects

A collection of objects describing the distinct areas of the saliency heat map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var salientObjects: [VNRectangleObservation]? { get }
```

## Discussion

The objects in this array don’t follow any specific ordering. It’s up to your app to iterate across the observations and apply desired ordering.

Requesting this array lazily computes the bounds of salient objects within the image.

