

- SwiftUI
- Image
-  init(decorative:variableValue:bundle:) 

Initializer

# init(decorative:variableValue:bundle:)

Creates an unlabeled, decorative image, with a variable value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    decorative name: String,
    variableValue: Double?,
    bundle: Bundle? = nil
)
```

## Parameters 

`name`  

The name of the image resource to lookup.

`variableValue`  

An optional value between `0.0` and `1.0` that the rendered image can use to customize its appearance, if specified. If the symbol doesn’t support variable values, this parameter has no effect.

`bundle`  

The bundle to search for the image resource. If `nil`, SwiftUI uses the main `Bundle`. Defaults to `nil`.

## Discussion

This initializer creates an image using a using a symbol in the specified bundle. The rendered symbol may alter its appearance to represent the value provided in `variableValue`.

Note

See WWDC22 session 10158: Adopt variable color in SF Symbols for details on how to create symbols that support variable values.

SwiftUI ignores this image for accessibility purposes.

## See Also

### Creating an image for decorative use

init(decorative: String, bundle: Bundle?)

Creates an unlabeled, decorative image.

init(decorative: CGImage, scale: CGFloat, orientation: Image.Orientation)

Creates an unlabeled, decorative image based on a Core Graphics image instance.

