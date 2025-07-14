

- Audio Toolbox
-  kAUGraphErr_InvalidAudioUnit 

Global Variable

# kAUGraphErr_InvalidAudioUnit

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAUGraphErr_InvalidAudioUnit: OSStatus { get }
```

## See Also

### Constants

var kAUGraphErr_CannotDoInCurrentContext: OSStatus

To avoid spinning or waiting in the render thread (a bad idea!), many of the calls to AUGraph can return: `kAUGraphErr_CannotDoInCurrentContext`. This result is only generated when you call an AUGraph API from its render callback. It means that the lock that it required was held at that time, by another thread. If you see this result code, you can generally attempt the action again - typically the NEXT render cycle (so in the mean time the lock can be cleared), or you can delegate that call to another thread in your app. You should not spin or put-to-sleep the render thread.

var kAUGraphErr_InvalidConnection: OSStatus

The attempted connection between two nodes cannot be made.

var kAUGraphErr_NodeNotFound: OSStatus

The specified node cannot be found.

var kAUGraphErr_OutputNodeErr: OSStatus

Audio processing graphs can only contain one output unit. This error is returned if trying to add a second output unit or if the graph’s output unit is removed while the graph is running.

