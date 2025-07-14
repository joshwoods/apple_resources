

- Media Accessibility
-  MAImageCaptioningCopyCaption(\_:\_:) 

Function

# MAImageCaptioningCopyCaption(\_:\_:)

Returns an accessibility caption from an image’s metadata.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func MAImageCaptioningCopyCaption(
    _ url: CFURL,
    _ error: UnsafeMutablePointer?
) -> CFString?
```

## See Also

### Image captioning settings

func MAImageCaptioningSetCaption(CFURL, CFString?, UnsafeMutablePointer&lt;CFError?>?) -> Bool

Sets the accessibility caption for an image’s metadata.

func MAImageCaptioningCopyMetadataTagPath() -> CFString

Returns the metadata tag path.

