

- Accessibility
- AXBrailleMap
-  present(\_:) 

Instance Method

# present(\_:)

Converts the data from the image you specify into the braille map.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 12.1+tvOS 15.2+visionOS 1.0+watchOS 8.2+

``` source
func present(_ image: CGImage)
```

## Parameters 

`image`  

An image to convert into the braille map.

## Discussion

Use this method to convert image data into the braille map directly, without the need to modify the heights of individual pins using setHeight(_:at:).

