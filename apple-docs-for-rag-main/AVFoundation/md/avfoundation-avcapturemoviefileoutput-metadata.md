

- AVFoundation
- AVCaptureMovieFileOutput
-  metadata 

Instance Property

# metadata

The metadata for the output file.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var metadata: [AVMetadataItem]? { get set }
```

## Discussion

This array contains AVMetadataItem objects. You use it to add metadata, such as copyright, creation date, and so on, to the recorded movie file.

## See Also

### Configuring movies

var movieFragmentInterval: CMTime

The number of seconds of output that are written per fragment.

