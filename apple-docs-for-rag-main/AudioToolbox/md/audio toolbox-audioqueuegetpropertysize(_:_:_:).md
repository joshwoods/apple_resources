

- Audio Toolbox
-  AudioQueueGetPropertySize(\_:\_:\_:) 

Function

# AudioQueueGetPropertySize(\_:\_:\_:)

Gets the size of the value of an audio queue property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueGetPropertySize(
    _ inAQ: AudioQueueRef,
    _ inID: AudioQueuePropertyID,
    _ outDataSize: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue that has the property value whose size you want to get.

`inID`  

The ID of the property value whose size you want to get. See AudioQueuePropertyID.

`outDataSize`  

On output, the size of the requested property value.

## Return Value

A result code. See Result Codes.

## See Also

### Manipulating Audio Queue Properties

func AudioQueueGetProperty(AudioQueueRef, AudioQueuePropertyID, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets an audio queue property value.

func AudioQueueSetProperty(AudioQueueRef, AudioQueuePropertyID, UnsafeRawPointer, UInt32) -> OSStatus

Sets an audio queue property value.

func AudioQueueAddPropertyListener(AudioQueueRef, AudioQueuePropertyID, AudioQueuePropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Adds a property listener callback to an audio queue.

func AudioQueueRemovePropertyListener(AudioQueueRef, AudioQueuePropertyID, AudioQueuePropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Removes a property listener callback from an audio queue.

