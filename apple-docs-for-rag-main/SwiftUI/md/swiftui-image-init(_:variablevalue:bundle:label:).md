

- SwiftUI
- Image
-  init(\_:variableValue:bundle:label:) 

Initializer

# init(\_:variableValue:bundle:label:)

Creates a labeled image that you can use as content for controls, with the specified label and variable value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ name: String,
    variableValue: Double?,
    bundle: Bundle? = nil,
    label: Text
)
```

## Parameters 

`name`  

The name of the image resource to lookup.

`variableValue`  

An optional value between `0.0` and `1.0` that the rendered image can use to customize its appearance, if specified. If the symbol doesn’t support variable values, this parameter has no effect.

`bundle`  

The bundle to search for the image resource. If `nil`, SwiftUI uses the main `Bundle`. Defaults to `nil`.

`label`  

The label associated with the image. SwiftUI uses the label for accessibility.

## Discussion

This initializer creates an image using a using a symbol in the specified bundle. The rendered symbol may alter its appearance to represent the value provided in `variableValue`.

Note

See WWDC22 session 10158: Adopt variable color in SF Symbols for details on how to create symbols that support variable values.

## See Also

### Creating an image for use as a control

init(String, bundle: Bundle?, label: Text)

Creates a labeled image that you can use as content for controls, with the specified label.

init(CGImage, scale: CGFloat, orientation: Image.Orientation, label: Text)

Creates a labeled image based on a Core Graphics image instance, usable as content for controls.

