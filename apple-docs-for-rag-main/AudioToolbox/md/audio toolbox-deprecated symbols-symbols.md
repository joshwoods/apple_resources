

- Audio Toolbox
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Inter-App Audio

Inter-App Audio is deprecated in iOS 13 and is unavailable when running iPad apps in macOS.

func AudioOutputUnitPublish(UnsafePointer&lt;AudioComponentDescription>, CFString, UInt32, AudioUnit) -> OSStatus

Registers an audio output unit for use by other applications.

Deprecated

func AudioOutputUnitGetHostIcon(AudioUnit, Float) -> UIImage?

The host app’s icon.

Deprecated

func AudioComponentGetIcon(AudioComponent, Float) -> UIImage?

The UIImage of the audio component’s icon.

Deprecated

func AudioComponentGetLastActiveTime(AudioComponent) -> CFAbsoluteTime

The time at which the application publishing the component was last active.

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

func AudioSessionRemovePropertyListener(AudioSessionPropertyID) -> OSStatus

Removes an audio session property listener callback function.

Deprecated

func AudioSessionRemovePropertyListenerWithUserData(AudioSessionPropertyID, AudioSessionPropertyListener!, UnsafeMutableRawPointer!) -> OSStatus

Removes a property listener callback function from your application’s audio session object.

Deprecated

func AudioSessionSetActive(Bool) -> OSStatus

Actives or deactivates your application’s audio session.

Deprecated

func AudioSessionSetActiveWithFlags(Bool, UInt32) -> OSStatus

Activates or deactivates your application’s audio session; provides flags for use by other audio sessions.

Deprecated

func AudioSessionSetProperty(AudioSessionPropertyID, UInt32, UnsafeRawPointer!) -> OSStatus

Sets the value of a specified audio session property.

Deprecated

### Callbacks

typealias AudioSessionInterruptionListener

Invoked when an audio interruption in iOS begins or ends.

Deprecated

typealias AudioSessionPropertyListener

Invoked when an audio session property changes in iOS.

Deprecated

### Data Types

struct ExtendedControlEvent

typealias MIDIEndpointRef = MIDIObjectRef

A MIDI source or destination an entity owns.

typealias MagicCookieInfo

A structure holding magic cookie information.

Deprecated

typealias NoteInstanceID

typealias ReadBytesFDF

typealias ReadPacketDataFDF

typealias ReadPacketsFDF

typealias SetPropertyFDF

typealias SetUserDataFDF

typealias WriteBytesFDF

typealias WritePacketsFDF

typealias AudioSessionPropertyID

The data type for an audio session property identifier.

Deprecated

### Constants

Audio Unit Attenuation Properties

Audio Unit Instrument Errors

Anonymous

Anonymous

Audio Graph Errors

Audio Converter Property ID

Anonymous

Anonymous

Anonymous

Anonymous

Anonymous

Anonymous

Anonymous

Music Device Properties

3D Mixer Audio Unit Properties

Properties for the Apple 3D Mixer audio unit.

var kAudioSession_AudioRouteChangeKey_OldRoute: String

var AU_SUPPORT_INTERAPP_AUDIO: Int32

Hardware Codec Capabilities

A constant to determine which hardware codecs can be used.

Deprecated Audio Codec Properties

Deprecated Constants Used With kAudioCodecBitRateFormat

Deprecated Constants Used With kAudioCodecOutputPrecedence

Deprecated Constants Used With kAudioSettings_Hint

Deprecated Audio Session Categories

Deprecated category identifiers for audio sessions. Do not use for new development.

### Audio Graphs

Audio Unit Processing Graph Services

Audio Unit Processing Graph Services provide interfaces for representing a set of audio units, connections between their inputs and outputs, and callbacks used to provide inputs. It also enables the embedding of sub (or child) processing graphs within parent graphs to allow for a logical organization of parts of an overall signal chain.

