

- AVFoundation
- AVCaptionRegion
-  mutableCopy(with:) 

Instance Method

# mutableCopy(with:)

Creates a mutable copy of a caption region.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func mutableCopy(with zone: NSZone? = nil) -> Any
```

## Parameters 

`zone`  

The system ignores this parameter. Objective-C doesn’t no longer supports memory zones.

## Return Value

A copy of the region.

## Discussion

This method throws an exception if the caption region contains an identifier.

## See Also

### Processing Regions

func encode(with: NSCoder)

Encodes the region using the specified encoder.

func isEqual(Any) -> Bool

Returns a Boolean value that indicates whether an object equals another.

