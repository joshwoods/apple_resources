

- Audio Toolbox
-  AudioSessionInitialize(\_:\_:\_:\_:) Deprecated

Function

# AudioSessionInitialize(\_:\_:\_:\_:)

Initializes an iOS application’s audio session object.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func AudioSessionInitialize(
    _ inRunLoop: CFRunLoop!,
    _ inRunLoopMode: CFString!,
    _ inInterruptionListener: AudioSessionInterruptionListener!,
    _ inClientData: UnsafeMutableRawPointer!
) -> OSStatus
```

Deprecated

Deprecated in iOS 7.0.

## Parameters 

`inRunLoop`  

The run loop that the interruption listener callback should be run on. Pass `NULL` to use the main run loop.

`inRunLoopMode`  

The mode for the run loop that the interruption listener function will run on. Passing `NULL` is equivalent to passing `kCFRunLoopDefaultMode`.

`inInterruptionListener`  

The interruption listener callback function. The application’s audio session object invokes the callback when the session is interrupted and (if the application is still running) when the interruption ends. Can be `NULL`. See AudioSessionInterruptionListener.

`inClientData`  

Data that you would like to be passed to your interruption listener callback.

## Return Value

A result code. See Result Codes.

## Discussion

Your application must call this function before making any other Audio Session Services calls. You may activate and deactivate your audio session as needed (see AudioSessionSetActive(_:)), but should initialize it only once.

## See Also

### Functions

func AudioFileReadPackets(AudioFileID, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer?) -> OSStatus

Reads a fixed duration of audio data from an audio file.

Deprecated

func AudioComponentGetIcon(AudioComponent, Float) -> UIImage?

The UIImage of the audio component’s icon.

Deprecated

func AudioComponentGetLastActiveTime(AudioComponent) -> CFAbsoluteTime

The time at which the application publishing the component was last active.

Deprecated

func AudioHardwareServiceAddPropertyListener(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>!, AudioObjectPropertyListenerProc!, UnsafeMutableRawPointer!) -> OSStatus

Registers a HAL audio object property listener callback function to be invoked when a specified property changes.

Deprecated

func AudioHardwareServiceGetPropertyData(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>!, UInt32, UnsafeRawPointer!, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutableRawPointer!) -> OSStatus

Gets the value for a specified property.

Deprecated

func AudioHardwareServiceGetPropertyDataSize(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>!, UInt32, UnsafeRawPointer!, UnsafeMutablePointer&lt;UInt32>!) -> OSStatus

Gets the payload size for a given property.

Deprecated

func AudioHardwareServiceHasProperty(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>!) -> Bool

Queries a HAL audio object about whether or not it has a specified property.

Deprecated

func AudioHardwareServiceIsPropertySettable(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> OSStatus

Queries a HAL audio object about whether a specified property is settable.

Deprecated

func AudioHardwareServiceRemovePropertyListener(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>!, AudioObjectPropertyListenerProc!, UnsafeMutableRawPointer!) -> OSStatus

Unregisters a HAL audio object property listener callback function.

Deprecated

func AudioHardwareServiceSetPropertyData(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>!, UInt32, UnsafeRawPointer!, UInt32, UnsafeRawPointer!) -> OSStatus

Asks a HAL audio object to change the value of a specified property.

Deprecated

func AudioOutputUnitGetHostIcon(AudioUnit, Float) -> UIImage?

The host app’s icon.

Deprecated

func AudioOutputUnitPublish(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioUnit) -> OSStatus

Registers an audio output unit for use by other applications.

Deprecated

func AudioSessionAddPropertyListener(AudioSessionPropertyID, AudioSessionPropertyListener!, UnsafeMutableRawPointer!) -> OSStatus

Adds a property listener callback function to your application’s audio session object.

Deprecated

func AudioSessionGetProperty(AudioSessionPropertyID, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutableRawPointer!) -> OSStatus

Gets the value of a specified audio session property.

Deprecated

func AudioSessionGetPropertySize(AudioSessionPropertyID, UnsafeMutablePointer&lt;UInt32>!) -> OSStatus

Gets the size of the value for a specified audio session property.

Deprecated

