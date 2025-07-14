

- Core Media
- CMPackingType
-  CMPackingType.sideBySide 

Case

# CMPackingType.sideBySide

The video contains packed frames that have a left eye image on the left and right eye image on the right.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case sideBySide
```

## Discussion

For side-by-side packed frames, the width of a frame in video data is twice as wide as the video displayed.

## See Also

### Frame Arrangement

case none

Each frame contains only a single image, and isn’t frame-packed.

case overUnder

The video contains packed frames that have a left eye image on the top and right eye image on the bottom.

