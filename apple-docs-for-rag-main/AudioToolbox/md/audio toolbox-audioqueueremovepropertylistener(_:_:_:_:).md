

- Audio Toolbox
-  AudioQueueRemovePropertyListener(\_:\_:\_:\_:) 

Function

# AudioQueueRemovePropertyListener(\_:\_:\_:\_:)

Removes a property listener callback from an audio queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueRemovePropertyListener(
    _ inAQ: AudioQueueRef,
    _ inID: AudioQueuePropertyID,
    _ inProc: AudioQueuePropertyListenerProc,
    _ inUserData: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue that you want to remove a property listener callback from.

`inID`  

The ID of the property whose changes you no longer want to respond to. See AudioQueuePropertyID.

`inProc`  

The callback to be removed.

`inUserData`  

The same custom data for the property listener callback that you passed when calling AudioQueueAddPropertyListener(_:_:_:_:).

## Return Value

A result code. See Result Codes.

## See Also

### Manipulating Audio Queue Properties

func AudioQueueGetProperty(AudioQueueRef, AudioQueuePropertyID, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets an audio queue property value.

func AudioQueueSetProperty(AudioQueueRef, AudioQueuePropertyID, UnsafeRawPointer, UInt32) -> OSStatus

Sets an audio queue property value.

func AudioQueueGetPropertySize(AudioQueueRef, AudioQueuePropertyID, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the size of the value of an audio queue property.

func AudioQueueAddPropertyListener(AudioQueueRef, AudioQueuePropertyID, AudioQueuePropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Adds a property listener callback to an audio queue.

