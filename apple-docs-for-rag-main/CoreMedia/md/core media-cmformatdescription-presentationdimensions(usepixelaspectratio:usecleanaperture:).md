

- Core Media
- CMFormatDescription
-  presentationDimensions(usePixelAspectRatio:useCleanAperture:) 

Instance Method

# presentationDimensions(usePixelAspectRatio:useCleanAperture:)

Returns the dimensions to take the pixel aspect ratio or clean aperture into account.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func presentationDimensions(
    usePixelAspectRatio: Bool = true,
    useCleanAperture: Bool = true
) -> CGSize
```

## Parameters 

`usePixelAspectRatio`  

If `true`, the function computes the dimensions maintaining the pixel aspect ratio.

`useCleanAperture`  

If `true`, the function computes the dimensions using the clean aperture.

## See Also

### Working with Video Descriptions

func cleanAperture(originIsAtTopLeft: Bool) -> CGRect

Returns the clean aperture.

func matchesImageBuffer(CVImageBuffer) -> Bool

Returns a Boolean value that indicates whether the format description matches an image buffer.

