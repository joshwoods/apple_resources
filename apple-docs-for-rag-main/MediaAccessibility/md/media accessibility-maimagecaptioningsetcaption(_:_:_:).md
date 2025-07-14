

- Media Accessibility
-  MAImageCaptioningSetCaption(\_:\_:\_:) 

Function

# MAImageCaptioningSetCaption(\_:\_:\_:)

Sets the accessibility caption for an image’s metadata.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func MAImageCaptioningSetCaption(
    _ url: CFURL,
    _ string: CFString?,
    _ error: UnsafeMutablePointer?
) -> Bool
```

## See Also

### Image captioning settings

func MAImageCaptioningCopyCaption(CFURL, UnsafeMutablePointer&lt;CFError?>?) -> CFString?

Returns an accessibility caption from an image’s metadata.

func MAImageCaptioningCopyMetadataTagPath() -> CFString

Returns the metadata tag path.

