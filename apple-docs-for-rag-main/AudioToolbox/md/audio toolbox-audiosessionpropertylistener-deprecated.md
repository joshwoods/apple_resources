

- Audio Toolbox
-  AudioSessionPropertyListener Deprecated

Type Alias

# AudioSessionPropertyListener

Invoked when an audio session property changes in iOS.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
typealias AudioSessionPropertyListener = (UnsafeMutableRawPointer?, AudioSessionPropertyID, UInt32, UnsafeRawPointer?) -> Void
```

Deprecated

Deprecated in iOS 7.0.

## Parameters 

`inClientData`  

Data that you specified in the `inClientData` parameter of the AudioSessionAddPropertyListener(_:_:_:) function. Can be `NULL`.

`inID`  

The identifier for the audio session property whose value just changed. See Audio Session Property Identifiers.

`inDataSize`  

The size, in bytes, of the value of the changed property.

`inData`  

The new value of the changed property.

## Discussion

If you named your function `MyPropertyListener`, you would declare it like this:

### Discussion

You can register one or more property listener callbacks with your application’s audio session object by calling the AudioSessionAddPropertyListener(_:_:_:) function.

## See Also

### Callbacks

typealias AudioSessionInterruptionListener

Invoked when an audio interruption in iOS begins or ends.

Deprecated

