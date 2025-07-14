

- AVFoundation
- AVCaptureAudioFileOutput
-  metadata 

Instance Property

# metadata

A collection of metadata to be written to the receiver’s output files.

macOS 10.7+

``` source
var metadata: [AVMetadataItem] { get set }
```

## Discussion

The value of this property is an array of `AVMetadataItem` objects representing the collection of top-level metadata to be written in each output file. Only ID3 v2.2, v2.3, or v2.4 style metadata items are supported.

## See Also

### Configuring Output

var audioSettings: [String : Any]?

The settings used to decode or re-encode audio before it is output by the receiver.

