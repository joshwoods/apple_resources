

- Audio Toolbox
-  AudioQueueGetParameter(\_:\_:\_:) 

Function

# AudioQueueGetParameter(\_:\_:\_:)

Gets an audio queue parameter value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueGetParameter(
    _ inAQ: AudioQueueRef,
    _ inParamID: AudioQueueParameterID,
    _ outValue: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue that you want to get a parameter value from.

`inParamID`  

The ID of the parameter whose value you want to get. In OS X v10.5, audio queues have one parameter available: `kAudioQueueParam_Volume`, which controls playback gain. See Audio Queue Parameters

`outValue`  

On output, points to the current value of the specified parameter.

## Return Value

A result code. See Result Codes.

## Discussion

You can access the current parameter values for an audio queue at any time with this function. An audio queue parameter value is the sum of settings applied at buffer granularity, using the AudioQueueEnqueueBufferWithParameters(_:_:_:_:_:_:_:_:_:_:) function, and settings applied to the audio queue per se, using the AudioQueueSetParameter(_:_:_:) function.

## See Also

### Manipulating Audio Queue Parameters

func AudioQueueSetParameter(AudioQueueRef, AudioQueueParameterID, AudioQueueParameterValue) -> OSStatus

Sets a playback audio queue parameter value.

