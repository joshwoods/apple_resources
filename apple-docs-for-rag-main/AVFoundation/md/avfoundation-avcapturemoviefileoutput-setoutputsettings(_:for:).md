

- AVFoundation
- AVCaptureMovieFileOutput
-  setOutputSettings(\_:for:) 

Instance Method

# setOutputSettings(\_:for:)

Sets the options the output uses to encode media from the given connection while recording.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func setOutputSettings(
    _ outputSettings: [String : Any]?,
    for connection: AVCaptureConnection
)
```

## Parameters 

`outputSettings`  

A dictionary of output settings. Pass an empty dictionary to specify that the format of the media from the connection shouldn’t change before writing to the file. Pass `nil` to specify that the session preset determines output format.

`connection`  

The connection delivering the media to encode.

## Discussion

For details on output settings, see Video settings for video connections and Audio settings for audio connections.

On iOS, your output settings dictionary may only contain keys listed returned from the supportedOutputSettingsKeys(for:) method. If you specify any other key, the system throws an invalid argument exception. Additionally, the value you specify for AVVideoCodecKey should be present in the availableVideoCodecTypes array. If you specify AVVideoCompressionPropertiesKey, you must also specify a valid value for AVVideoCodecKey.

On iOS, the outputSettings(for:) method always provides a fully populated dictionary. If you call outputSettings(for:) with the intent of overriding a few of the values, you must exclude keys that aren’t supported before calling setOutputSettings(_:for:). When providing an AVVideoCompressionPropertiesKey sub dictionary, you may specify a sparse dictionary. A movie file output object always fills in missing keys with default values for the current capture session configuration.

## See Also

### Managing output settings

func supportedOutputSettingsKeys(for: AVCaptureConnection) -> [String]

Returns a list of supported keys to use in the output settings dictionary.

func outputSettings(for: AVCaptureConnection) -> [String : Any]

Returns the settings the output uses to encode media from the specified connection.

var availableVideoCodecTypes: [AVVideoCodecType]

The video codecs types the output supports for recording movie files.

