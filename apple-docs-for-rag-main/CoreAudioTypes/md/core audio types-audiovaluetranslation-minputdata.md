

- Core Audio Types
- AudioValueTranslation
-  mInputData 

Instance Property

# mInputData

The buffer containing the data to be translated.

iOS 2.0+iPadOS 2.0+macOS 10.1+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mInputData: UnsafeMutableRawPointer
```

## See Also

### Instance Properties

var mInputDataSize: UInt32

The number of bytes in the buffer pointed at by `mInputData`.

var mOutputData: UnsafeMutableRawPointer

The buffer to hold the result of the translation.

var mOutputDataSize: UInt32

The number of bytes in the buffer pointed at by `mOutputData`.

