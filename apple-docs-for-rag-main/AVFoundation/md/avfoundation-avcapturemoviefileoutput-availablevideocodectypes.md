

- AVFoundation
- AVCaptureMovieFileOutput
-  availableVideoCodecTypes 

Instance Property

# availableVideoCodecTypes

The video codecs types the output supports for recording movie files.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var availableVideoCodecTypes: [AVVideoCodecType] { get }
```

## Discussion

The first codec in this list is the default for recording movie files. To record using a different codec, call the setOutputSettings(_:for:) method, passing a video settings dictionary with a value for AVVideoCodecKey that matches one of the other values in this list.

## See Also

### Managing output settings

func supportedOutputSettingsKeys(for: AVCaptureConnection) -> [String]

Returns a list of supported keys to use in the output settings dictionary.

func outputSettings(for: AVCaptureConnection) -> [String : Any]

Returns the settings the output uses to encode media from the specified connection.

func setOutputSettings([String : Any]?, for: AVCaptureConnection)

Sets the options the output uses to encode media from the given connection while recording.

