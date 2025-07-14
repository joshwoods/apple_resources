

- Core Audio Types
- AudioValueTranslation
-  mInputDataSize 

Instance Property

# mInputDataSize

The number of bytes in the buffer pointed at by `mInputData`.

iOS 2.0+iPadOS 2.0+macOS 10.1+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mInputDataSize: UInt32
```

## See Also

### Instance Properties

var mInputData: UnsafeMutableRawPointer

The buffer containing the data to be translated.

var mOutputData: UnsafeMutableRawPointer

The buffer to hold the result of the translation.

var mOutputDataSize: UInt32

The number of bytes in the buffer pointed at by `mOutputData`.

