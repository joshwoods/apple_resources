

- Sound Analysis
-  SNError 

Structure

# SNError

An error from the Sound Analysis framework.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SNError
```

## Topics

### Error Codes

static var invalidModel: SNError.Code

An error that indicates the sound classifier’s underlying Core ML model is an invalid model type.

static var invalidFormat: SNError.Code

An error that indicates the audio data’s format isn’t valid.

static var invalidFile: SNError.Code

An error that indicates an audio file is invalid.

static var operationFailed: SNError.Code

An error that occurs when the framework fails to analyze audio.

static var unknownError: SNError.Code

An error that represents a failure that no other error handles.

### Error Information

enum Code

The enumerated error codes that the Sound Analysis framework produces.

### Error Domain

let SNErrorDomain: String

A string that identifies the Sound Analysis error domain.

static var errorDomain: String

A statically accessible string that identifies the Sound Analysis error domain.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

The enumerated error codes that the Sound Analysis framework produces.

let SNErrorDomain: String

A string that identifies the Sound Analysis error domain.

