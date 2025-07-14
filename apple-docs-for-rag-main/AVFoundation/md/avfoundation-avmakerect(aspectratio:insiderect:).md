

- AVFoundation
-  AVMakeRect(aspectRatio:insideRect:) 

Function

# AVMakeRect(aspectRatio:insideRect:)

Returns a scaled rectangle that maintains the specified aspect ratio within a bounding rectangle.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AVMakeRect(
    aspectRatio: CGSize,
    insideRect boundingRect: CGRect
) -> CGRect
```

## Parameters 

`aspectRatio`  

The width and height ratio (aspect ratio) you want to maintain.

`boundingRect`  

The bounding rectangle you want to fit into.

## Return Value

Returns a scaled `CGRect` that maintains the aspect ratio specified by `aspectRatio` that fits within `boundingRect`.

## Discussion

Use this function when attempting to fit the presentation size of a player item object’s content within the bounds of another CALayer. Use the returned CGRect as the player layer’s frame property value. For example:

- Swift
- Objective-C

```
let aspectRatio = CGSize(width: 1920, height: 1080)
playerLayer.frame = AVMakeRect(aspectRatio: aspectRatio, insideRect: superLayer.bounds)
```

```
CGSize aspectRatio = CGSizeMake(1920, 1080);
self.playerLayer.frame = AVMakeRectWithAspectRatioInsideRect(aspectRatio, self.superLayer.bounds);
```

