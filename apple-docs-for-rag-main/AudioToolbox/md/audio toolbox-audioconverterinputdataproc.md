

- Audio Toolbox
-  AudioConverterInputDataProc 

Type Alias

# AudioConverterInputDataProc

Deprecated. Use AudioConverterFillComplexBuffer(_:_:_:_:_:_:) instead.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioConverterInputDataProc = (AudioConverterRef, UnsafeMutablePointer, UnsafeMutablePointer, UnsafeMutableRawPointer?) -> OSStatus
```

## Discussion

If you named your callback function `MyAudioConverterInputDataProc`, you would declare it like this:

### Discussion

This deprecated callback supplies input data to the AudioConverterFillBuffer function. Use AudioConverterComplexInputDataProc instead.

## See Also

### Callbacks

typealias AudioConverterComplexInputDataProc

Supplies input data to the AudioConverterFillComplexBuffer(_:_:_:_:_:_:) function.

