

- Audio Toolbox
-  AudioQueueSetProperty(\_:\_:\_:\_:) 

Function

# AudioQueueSetProperty(\_:\_:\_:\_:)

Sets an audio queue property value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueSetProperty(
    _ inAQ: AudioQueueRef,
    _ inID: AudioQueuePropertyID,
    _ inData: UnsafeRawPointer,
    _ inDataSize: UInt32
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue that you want to set a property value on.

`inID`  

The ID of the property whose value you want to set. See AudioQueuePropertyID.

`inData`  

The property value to set.

`inDataSize`  

The size of the property data.

## Return Value

A result code. See Result Codes.

## See Also

### Manipulating Audio Queue Properties

func AudioQueueGetProperty(AudioQueueRef, AudioQueuePropertyID, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets an audio queue property value.

func AudioQueueGetPropertySize(AudioQueueRef, AudioQueuePropertyID, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the size of the value of an audio queue property.

func AudioQueueAddPropertyListener(AudioQueueRef, AudioQueuePropertyID, AudioQueuePropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Adds a property listener callback to an audio queue.

func AudioQueueRemovePropertyListener(AudioQueueRef, AudioQueuePropertyID, AudioQueuePropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Removes a property listener callback from an audio queue.

