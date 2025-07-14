

- MusicKit
- ArtworkImage
-  init(\_:width:) 

Initializer

# init(\_:width:)

Creates an instance with a specified width.

MusicKitSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
init(
    _ artwork: Artwork,
    width: CGFloat
)
```

## Discussion

This initializer derives the URL for loading the artwork image from the Artwork instance and the specified sizing parameters, as well as the display scale for the current environment.

The loaded image and placeholder have constrained frames from these sizing parameters.

If you provide the width only, the artwork image calculates the height dimension as a proportional length according to the aspect ratio of the artwork.

