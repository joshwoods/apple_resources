

- Audio Toolbox
-  AudioQueuePropertyListenerProc 

Type Alias

# AudioQueuePropertyListenerProc

Called by the system when a specified audio queue property changes value.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioQueuePropertyListenerProc = (UnsafeMutableRawPointer?, AudioQueueRef, AudioQueuePropertyID) -> Void
```

## Parameters 

`inUserData`  

The custom data you’ve specified in the `inUserData` parameter of the AudioQueueAddPropertyListener(_:_:_:_:) function.

`inAQ`  

The recording or playback audio queue that invoked the callback.

`inID`  

The ID of the property whose value changes you want to observe.

## Discussion

If you name your callback function `MyAudioQueuePropertyListenerProc`, you would declare it like this:

### Discussion

Install this callback in an audio queue by calling the AudioQueueAddPropertyListener(_:_:_:_:) function. For example, say you want your application to be notified, after you call the AudioQueueStop(_:_:) function with the `inImmedate` parameter set to `false`, that audio has finished playing. Perform these steps:

1.  Define this property listener callback function to listen for changes to the kAudioQueueProperty_IsRunning property.

2.  Install this callback, using the AudioQueueAddPropertyListener(_:_:_:_:) function, in the playback audio queue that you want to monitor.

## See Also

### Callbacks

typealias AudioQueueInputCallback

Called by the system when a recording audio queue has finished filling an audio queue buffer.

typealias AudioQueueOutputCallback

Called by the system when an audio queue buffer is available for reuse.

