

- SwiftUI
- Image
-  init(decorative:bundle:) 

Initializer

# init(decorative:bundle:)

Creates an unlabeled, decorative image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    decorative name: String,
    bundle: Bundle? = nil
)
```

## Parameters 

`name`  

The name of the image resource to lookup

`bundle`  

The bundle to search for the image resource. If `nil`, SwiftUI uses the main `Bundle`. Defaults to `nil`.

## Discussion

SwiftUI ignores this image for accessibility purposes.

## See Also

### Creating an image for decorative use

init(decorative: String, variableValue: Double?, bundle: Bundle?)

Creates an unlabeled, decorative image, with a variable value.

init(decorative: CGImage, scale: CGFloat, orientation: Image.Orientation)

Creates an unlabeled, decorative image based on a Core Graphics image instance.

