

- Audio Toolbox
-  AudioQueueSetParameter(\_:\_:\_:) 

Function

# AudioQueueSetParameter(\_:\_:\_:)

Sets a playback audio queue parameter value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueSetParameter(
    _ inAQ: AudioQueueRef,
    _ inParamID: AudioQueueParameterID,
    _ inValue: AudioQueueParameterValue
) -> OSStatus
```

## Parameters 

`inAQ`  

The playback audio queue that you want to set a parameter value on.

`inParamID`  

The ID of the parameter you want to set. In OS X v10.5, audio queues have one parameter available: `kAudioQueueParam_Volume`, which controls playback gain. See Audio Queue Parameters.

`inValue`  

The parameter value to set.

## Return Value

A result code. See Result Codes.

## Discussion

Use this function to change the settings for a playback audio queue directly. Changes take effect immediately. To set playback gain at the granularity of an audio queue buffer, use the AudioQueueEnqueueBufferWithParameters(_:_:_:_:_:_:_:_:_:_:) function.

## See Also

### Related Documentation

func AudioQueueEnqueueBufferWithParameters(AudioQueueRef, AudioQueueBufferRef, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, UInt32, UInt32, UInt32, UnsafePointer&lt;AudioQueueParameterEvent>?, UnsafePointer&lt;AudioTimeStamp>?, UnsafeMutablePointer&lt;AudioTimeStamp>?) -> OSStatus

Adds a buffer to the buffer queue of a playback audio queue object, specifying start time and other settings.

### Manipulating Audio Queue Parameters

func AudioQueueGetParameter(AudioQueueRef, AudioQueueParameterID, UnsafeMutablePointer&lt;AudioQueueParameterValue>) -> OSStatus

Gets an audio queue parameter value.

