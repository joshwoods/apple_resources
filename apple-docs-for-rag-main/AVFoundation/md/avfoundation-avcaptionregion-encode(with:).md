

- AVFoundation
- AVCaptionRegion
-  encode(with:) 

Instance Method

# encode(with:)

Encodes the region using the specified encoder.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func encode(with encoder: NSCoder)
```

## Parameters 

`encoder`  

An encoder instance to use.

## Discussion

This method throws an exception if the caption region’s size has different units for width and height, or if the units are unrecognizeable.

## See Also

### Processing Regions

func mutableCopy(with: NSZone?) -> Any

Creates a mutable copy of a caption region.

func isEqual(Any) -> Bool

Returns a Boolean value that indicates whether an object equals another.

