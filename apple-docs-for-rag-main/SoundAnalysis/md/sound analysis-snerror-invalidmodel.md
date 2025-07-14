

- Sound Analysis
- SNError
-  invalidModel 

Type Property

# invalidModel

An error that indicates the sound classifier’s underlying Core ML model is an invalid model type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var invalidModel: SNError.Code { get }
```

## See Also

### Error Codes

static var invalidFormat: SNError.Code

An error that indicates the audio data’s format isn’t valid.

static var invalidFile: SNError.Code

An error that indicates an audio file is invalid.

static var operationFailed: SNError.Code

An error that occurs when the framework fails to analyze audio.

static var unknownError: SNError.Code

An error that represents a failure that no other error handles.

