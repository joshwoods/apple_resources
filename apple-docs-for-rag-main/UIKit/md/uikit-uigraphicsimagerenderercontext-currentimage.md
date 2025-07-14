

- UIKit
- UIGraphicsImageRendererContext
-  currentImage 

Instance Property

# currentImage

The current state of the drawing context, expressed as an object that manages image data in your app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var currentImage: UIImage { get }
```

## Discussion

Use this property to access the current Core Graphics context as a UIImage object while providing drawing instructions for one of the drawing methods in UIGraphicsImageRenderer.

