

- AVFoundation
- AVMutableMovieTrack
-  replaceFormatDescription(\_:with:) 

Instance Method

# replaceFormatDescription(\_:with:)

Replaces the track’s format description with a new format description.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 6.0+

``` source
func replaceFormatDescription(
    _ formatDescription: CMFormatDescription,
    with newFormatDescription: CMFormatDescription
)
```

## Parameters 

`formatDescription`  

The CMFormatDescription object to be replaced.

`newFormatDescription`  

The CMFormatDescription object to replacing the specified format description.

## Discussion

Use this method to change a track’s format descriptions, such as adding format description extensions to a format description or changing the audio channel layout of an audio track. Format description can have extensions of type kCMFormatDescriptionExtension_VerbatimSampleDescription and kCMFormatDescriptionExtension_VerbatimISOSampleEntry. If you modify a copy of a format description, delete those extensions from the copy or your changes might be ignored.

## See Also

### Changing Format Descriptions

var formatDescriptions: [Any]

The format descriptions of the media samples that a track references.

