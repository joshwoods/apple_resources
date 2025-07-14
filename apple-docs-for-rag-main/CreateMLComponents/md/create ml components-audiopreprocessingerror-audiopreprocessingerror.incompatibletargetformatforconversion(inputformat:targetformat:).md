

- Create ML Components
- AudioPreprocessingError
-  AudioPreprocessingError.incompatibleTargetFormatForConversion(inputFormat:targetFormat:) 

Case

# AudioPreprocessingError.incompatibleTargetFormatForConversion(inputFormat:targetFormat:)

An error that indicates that the input and output formats are incompatible for creating an audio converter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case incompatibleTargetFormatForConversion(
    inputFormat: AVAudioFormat,
    targetFormat: AVAudioFormat
)
```

## See Also

### Analyzing the error

var errorDescription: String?

A localized message describing what error occurred.

