

- Audio Toolbox
-  AudioFileReadPackets(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# AudioFileReadPackets(\_:\_:\_:\_:\_:\_:\_:)

Reads a fixed duration of audio data from an audio file.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func AudioFileReadPackets(
    _ inAudioFile: AudioFileID,
    _ inUseCache: Bool,
    _ outNumBytes: UnsafeMutablePointer,
    _ outPacketDescriptions: UnsafeMutablePointer?,
    _ inStartingPacket: Int64,
    _ ioNumPackets: UnsafeMutablePointer,
    _ outBuffer: UnsafeMutableRawPointer?
) -> OSStatus
```

Deprecated

no longer supported

## Parameters 

`inAudioFile`  

The audio file whose audio packets you want to read.

`inUseCache`  

Set to `true` to cache the data. Otherwise, set to `false`.

`outNumBytes`  

On output, the number of bytes actually read.

`outPacketDescriptions`  

On output, an array of packet descriptions for the packets that were read. The array that you pass must be large enough to accommodate descriptions for the number of packets requested in the `ioNumPackets` parameter.

This parameter applies only to variable bit-rate data. If the file being read contains constant bit-rate (CBR) data, such as linear PCM, this parameter does not get filled. Pass `NULL` if the file’s data format is CBR.

`inStartingPacket`  

The packet index of the first packet you want to read.

`ioNumPackets`  

On input, the number of packets to read. On output, the number of packets actually read.

You will see a difference in the input and output values when this function has reached the end of the file you are reading. In this case, the output value for this parameter is smaller than its input value.

`outBuffer`  

Memory that you allocate to hold the read packets. Determine an appropriate size by multiplying the number of packets requested (in the `ioNumPackets` parameter) by the maximum (or upper bound for) packet size of the audio file. For uncompressed audio formats, a packet is equal to a frame.

## Return Value

A result code. See Result Codes.

## Discussion

If you do not need to read a fixed duration of audio data, but rather want to use your memory buffer most efficiently, use AudioFileReadPacketData(_:_:_:_:_:_:_:) instead of this function.

When reading variable bit-rate (VBR) audio data, using this function requires that you allocate more memory than you would for the AudioFileReadPacketData(_:_:_:_:_:_:_:) function. See the descriptions for the `outBuffer` parameter in each of these two functions.

In addition, this function is less efficient than AudioFileReadPacketData(_:_:_:_:_:_:_:) when reading compressed file formats that do not have packet tables, such as MP3 or ADTS. Use this function only when you need to read a fixed duration of audio data, or when you are reading only uncompressed audio.

Audio File Services reads one 32-bit chunk of a file at a time.

## See Also

### Related Documentation

func AudioFileWritePackets(AudioFileID, Bool, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

Writes packets of audio data to an audio data file.

### Functions

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

func AudioSessionInitialize(CFRunLoop!, CFString!, AudioSessionInterruptionListener!, UnsafeMutableRawPointer!) -> OSStatus

Initializes an iOS application’s audio session object.

Deprecated

