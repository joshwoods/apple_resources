

- Core Audio Types
-  AudioValueTranslation 

Structure

# AudioValueTranslation

A structure that stores buffers to use in translation operations.

iOS 2.0+iPadOS 2.0+macOS 10.1+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct AudioValueTranslation
```

## Topics

### Initializers

init(mInputData: UnsafeMutableRawPointer, mInputDataSize: UInt32, mOutputData: UnsafeMutableRawPointer, mOutputDataSize: UInt32)

### Instance Properties

var mInputData: UnsafeMutableRawPointer

The buffer containing the data to be translated.

var mInputDataSize: UInt32

The number of bytes in the buffer pointed at by `mInputData`.

var mOutputData: UnsafeMutableRawPointer

The buffer to hold the result of the translation.

var mOutputDataSize: UInt32

The number of bytes in the buffer pointed at by `mOutputData`.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Values

struct AudioValueRange

A structure that represents a continuous range of values.

