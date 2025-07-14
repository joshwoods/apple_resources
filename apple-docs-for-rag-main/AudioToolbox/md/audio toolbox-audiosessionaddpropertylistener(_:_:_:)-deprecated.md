

- Audio Toolbox
-  AudioSessionAddPropertyListener(\_:\_:\_:) Deprecated

Function

# AudioSessionAddPropertyListener(\_:\_:\_:)

Adds a property listener callback function to your application’s audio session object.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func AudioSessionAddPropertyListener(
    _ inID: AudioSessionPropertyID,
    _ inProc: AudioSessionPropertyListener!,
    _ inClientData: UnsafeMutableRawPointer!
) -> OSStatus
```

Deprecated

Deprecated in iOS 7.0.

## Parameters 

`inID`  

The identifier for the audio session property whose value changes you want to listen for.

`inProc`  

The name of your property listener callback function.

`inClientData`  

Data that you would like to be passed to your property listener callback.

## Return Value

A result code. See Result Codes.

## Discussion

When an audio session property value changes, and you have added a listener callback for that property, the audio session object invokes the callback.

You can add exactly one listener callback for a given `inID`-`inClientData` pair. In other words, you can add more than one property listener callback function for a given audio session property, provided you pass a unique `inClientData` parameter value each time you add a property listener.

Audio session properties are listed and described in Audio Session Property Identifiers.

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

func AudioSessionGetProperty(AudioSessionPropertyID, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutableRawPointer!) -> OSStatus

Gets the value of a specified audio session property.

Deprecated

func AudioSessionGetPropertySize(AudioSessionPropertyID, UnsafeMutablePointer&lt;UInt32>!) -> OSStatus

Gets the size of the value for a specified audio session property.

Deprecated

func AudioSessionInitialize(CFRunLoop!, CFString!, AudioSessionInterruptionListener!, UnsafeMutableRawPointer!) -> OSStatus

Initializes an iOS application’s audio session object.

Deprecated

