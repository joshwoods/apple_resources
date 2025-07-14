

- AVFoundation
- AVCaptureMovieFileOutput
-  supportedOutputSettingsKeys(for:) 

Instance Method

# supportedOutputSettingsKeys(for:)

Returns a list of supported keys to use in the output settings dictionary.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func supportedOutputSettingsKeys(for connection: AVCaptureConnection) -> [String]
```

## Parameters 

`connection`  

The connection that delivers the media to encode.

## Return Value

An array of keys that can be set in the setOutputSettings(_:for:)method.

## See Also

### Managing output settings

func outputSettings(for: AVCaptureConnection) -> [String : Any]

Returns the settings the output uses to encode media from the specified connection.

func setOutputSettings([String : Any]?, for: AVCaptureConnection)

Sets the options the output uses to encode media from the given connection while recording.

var availableVideoCodecTypes: [AVVideoCodecType]

The video codecs types the output supports for recording movie files.

