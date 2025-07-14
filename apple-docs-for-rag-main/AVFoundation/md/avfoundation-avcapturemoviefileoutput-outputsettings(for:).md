

- AVFoundation
- AVCaptureMovieFileOutput
-  outputSettings(for:) 

Instance Method

# outputSettings(for:)

Returns the settings the output uses to encode media from the specified connection.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func outputSettings(for connection: AVCaptureConnection) -> [String : Any]
```

## Parameters 

`connection`  

The connection delivering the media to encode.

## Return Value

A dictionary of output settings.

## Discussion

If the returned value is an empty dictionary, the format of the media from the connection isn’t changed before writing to the file.

If you call setOutputSettings(_:for:) with a `nil` dictionary, this method returns a non-`nil` dictionary that reflects the settings used by the capture session’s sessionPreset value.

## See Also

### Managing output settings

func supportedOutputSettingsKeys(for: AVCaptureConnection) -> [String]

Returns a list of supported keys to use in the output settings dictionary.

func setOutputSettings([String : Any]?, for: AVCaptureConnection)

Sets the options the output uses to encode media from the given connection while recording.

var availableVideoCodecTypes: [AVVideoCodecType]

The video codecs types the output supports for recording movie files.

