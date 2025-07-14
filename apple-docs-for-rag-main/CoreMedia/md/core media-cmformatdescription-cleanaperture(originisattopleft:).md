

- Core Media
- CMFormatDescription
-  cleanAperture(originIsAtTopLeft:) 

Instance Method

# cleanAperture(originIsAtTopLeft:)

Returns the clean aperture.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func cleanAperture(originIsAtTopLeft: Bool) -> CGRect
```

## Parameters 

`originIsAtTopLeft`  

If `true`, the origin begins at the top-left corner of the rectangle instead of the bottom-left.

## See Also

### Working with Video Descriptions

func matchesImageBuffer(CVImageBuffer) -> Bool

Returns a Boolean value that indicates whether the format description matches an image buffer.

func presentationDimensions(usePixelAspectRatio: Bool, useCleanAperture: Bool) -> CGSize

Returns the dimensions to take the pixel aspect ratio or clean aperture into account.

