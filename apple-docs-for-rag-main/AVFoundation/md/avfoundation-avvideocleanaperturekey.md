

- AVFoundation
-  AVVideoCleanApertureKey 

Global Variable

# AVVideoCleanApertureKey

A key that defines the region within the video dimension displayed during playback.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
let AVVideoCleanApertureKey: String
```

## Discussion

The value for this key is an instance of `NSDictionary` containing one or more of the following keys: AVVideoCleanApertureWidthKey, AVVideoCleanApertureHeightKey, AVVideoCleanApertureHorizontalOffsetKey, or AVVideoCleanApertureVerticalOffsetKey. If no clean aperture region is specified, the playback displays the entire frame.

## See Also

### Clean aperture

let AVVideoCleanApertureWidthKey: String

A key to access the width of video that’s free from transition artifacts caused by signal encoding.

let AVVideoCleanApertureHeightKey: String

A key to access the height of video that’s free from transition artifacts caused by signal encoding.

let AVVideoCleanApertureVerticalOffsetKey: String

A key to access the vertical offset of video that’s free from transition artifacts caused by signal encoding.

let AVVideoCleanApertureHorizontalOffsetKey: String

A key to access the horizontal offset of video that’s free from transition artifacts caused by signal encoding.

