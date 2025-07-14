

- SwiftUI
- Image
-  resizable(capInsets:resizingMode:) 

Instance Method

# resizable(capInsets:resizingMode:)

Sets the mode by which SwiftUI resizes an image to fit its space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func resizable(
    capInsets: EdgeInsets = EdgeInsets(),
    resizingMode: Image.ResizingMode = .stretch
) -> Image
```

## Parameters 

`capInsets`  

Inset values that indicate a portion of the image that SwiftUI doesn’t resize.

`resizingMode`  

The mode by which SwiftUI resizes the image.

## Return Value

An image, with the new resizing behavior set.

## Mentioned in 

Fitting images into available space

