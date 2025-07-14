

- Audio Toolbox
-  AudioSessionInterruptionListener Deprecated

Type Alias

# AudioSessionInterruptionListener

Invoked when an audio interruption in iOS begins or ends.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
typealias AudioSessionInterruptionListener = (UnsafeMutableRawPointer?, UInt32) -> Void
```

Deprecated

Deprecated in iOS 7.0.

## Parameters 

`inClientData`  

Data that you specified in the `inClientData` parameter of the AudioSessionInitialize(_:_:_:_:) function. Can be `NULL`.

`inInterruptionState`  

A constant that indicates whether the interruption has just started or just ended. See Audio Session Interruption States.

## Discussion

If you named your function `MyInterruptionListener`, you would declare it like this:

### Discussion

To register your interruption listener callback with your application’s audio session object, specify it in the AudioSessionInitialize(_:_:_:_:) function.

## See Also

### Callbacks

typealias AudioSessionPropertyListener

Invoked when an audio session property changes in iOS.

Deprecated

