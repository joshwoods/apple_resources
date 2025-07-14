

- Audio Toolbox
-  AudioQueueGetProperty(\_:\_:\_:\_:) 

Function

# AudioQueueGetProperty(\_:\_:\_:\_:)

Gets an audio queue property value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueGetProperty(
    _ inAQ: AudioQueueRef,
    _ inID: AudioQueuePropertyID,
    _ outData: UnsafeMutableRawPointer,
    _ ioDataSize: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue that you want to get a property value from.

`inID`  

The ID of the property whose value you want to get. See AudioQueuePropertyID.

`outData`  

On output, the desired property value.

`ioDataSize`  

On input, the maximum bytes of space the caller expects to receive. On output, the actual data size of the property value.

## Return Value

A result code. See Result Codes.

## Discussion

Before calling this function, you can use the AudioQueueGetPropertySize(_:_:_:) function to determine the size, in bytes, of the value of a specified property. Some properties have values of a specific size, as described in AudioQueuePropertyID.

### Special Considerations

Some Core Audio property values are C types and others are Core Foundation objects.

If you call this function to retrieve a value that is a Core Foundation object, then this function—despite the use of “Get” in its name—duplicates the object. You are responsible for releasing the object, as described in The Create Rule in Memory Management Programming Guide for Core Foundation.

## See Also

### Manipulating Audio Queue Properties

func AudioQueueSetProperty(AudioQueueRef, AudioQueuePropertyID, UnsafeRawPointer, UInt32) -> OSStatus

Sets an audio queue property value.

func AudioQueueGetPropertySize(AudioQueueRef, AudioQueuePropertyID, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the size of the value of an audio queue property.

func AudioQueueAddPropertyListener(AudioQueueRef, AudioQueuePropertyID, AudioQueuePropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Adds a property listener callback to an audio queue.

func AudioQueueRemovePropertyListener(AudioQueueRef, AudioQueuePropertyID, AudioQueuePropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Removes a property listener callback from an audio queue.

