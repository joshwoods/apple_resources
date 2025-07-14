

- Core Media
- CMFormatDescription
-  matchesImageBuffer(\_:) 

Instance Method

# matchesImageBuffer(\_:)

Returns a Boolean value that indicates whether the format description matches an image buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func matchesImageBuffer(_ imageBuffer: CVImageBuffer) -> Bool
```

## Parameters 

`imageBuffer`  

The image buffer to validate against.

## See Also

### Working with Video Descriptions

func cleanAperture(originIsAtTopLeft: Bool) -> CGRect

Returns the clean aperture.

func presentationDimensions(usePixelAspectRatio: Bool, useCleanAperture: Bool) -> CGSize

Returns the dimensions to take the pixel aspect ratio or clean aperture into account.

