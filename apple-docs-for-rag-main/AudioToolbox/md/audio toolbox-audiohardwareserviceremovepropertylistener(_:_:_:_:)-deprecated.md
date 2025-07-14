

- Audio Toolbox
-  AudioHardwareServiceRemovePropertyListener(\_:\_:\_:\_:) Deprecated

Function

# AudioHardwareServiceRemovePropertyListener(\_:\_:\_:\_:)

Unregisters a HAL audio object property listener callback function.

macOS 10.5–10.11Deprecated

``` source
func AudioHardwareServiceRemovePropertyListener(
    _ inObjectID: AudioObjectID,
    _ inAddress: UnsafePointer!,
    _ inListener: AudioObjectPropertyListenerProc!,
    _ inClientData: UnsafeMutableRawPointer!
) -> OSStatus
```

Deprecated

no longer supported

## Parameters 

`inObjectID`  

The HAL audio object to unregister the listener callback function from.

`inAddress`  

The property you no longer want notifications about.

`inListener`  

The property listener callback function you are removing.

`inClientData`  

Application data you had specified when registering the callback function.

## Return Value

A result code.

## See Also

### Related Documentation

func AudioHardwareServiceAddPropertyListener(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>!, AudioObjectPropertyListenerProc!, UnsafeMutableRawPointer!) -> OSStatus

Registers a HAL audio object property listener callback function to be invoked when a specified property changes.

Deprecated

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

func AudioSessionInitialize(CFRunLoop!, CFString!, AudioSessionInterruptionListener!, UnsafeMutableRawPointer!) -> OSStatus

Initializes an iOS application’s audio session object.

Deprecated

