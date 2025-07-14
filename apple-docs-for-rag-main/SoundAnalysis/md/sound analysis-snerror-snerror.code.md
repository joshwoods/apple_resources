

- Sound Analysis
- SNError
-  SNError.Code 

Enumeration

# SNError.Code

The enumerated error codes that the Sound Analysis framework produces.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Code
```

## Topics

### Errors

case invalidModel

An error that indicates the sound classifier’s underlying Core ML model is an invalid model type.

case invalidFormat

An error that indicates the audio data’s format isn’t valid.

case invalidFile

An error that indicates an audio file is invalid.

case operationFailed

An error that occurs when the framework fails to analyze audio.

case unknownError

An error that represents a failure that no other error handles.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct SNError

An error from the Sound Analysis framework.

let SNErrorDomain: String

A string that identifies the Sound Analysis error domain.

