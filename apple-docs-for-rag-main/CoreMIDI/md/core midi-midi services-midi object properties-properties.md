

- Core MIDI
- MIDI Services
-  MIDI Object Properties 

API Collection

# MIDI Object Properties

Configure the properties of MIDI objects.

## Topics

### Identification

let kMIDIPropertyName: CFString

A name for a device, entity, or endpoint.

let kMIDIPropertyModel: CFString

The model name of a device or endpoint.

let kMIDIPropertyManufacturer: CFString

The manufacturer name of a device or endpoint.

let kMIDIPropertyUniqueID: CFString

The unique identifier of a device, entity, or, endpoint.

let kMIDIPropertyDeviceID: CFString

The user-visible System Exclusive (SysEx) identifier of a device or entity.

### Capabilities

let kMIDIPropertySupportsMMC: CFString

A Boolean value that indicates whether the device or entity implements the MIDI Machine Control portion of the MIDI specification.

let kMIDIPropertySupportsGeneralMIDI: CFString

A Boolean value that indicates whether the device or entity implements the General MIDI specification.

let kMIDIPropertySupportsShowControl: CFString

A Boolean value that indicates whether the device implements the MIDI Show Control specification.

### Configuration

let kMIDIPropertyNameConfigurationDictionary: CFString

The device’s current patch, note, and control name values in MIDINameDocument XML format.

let kMIDIPropertyMaxSysExSpeed: CFString

The maximum rate, in bytes per second, at which the system may reliably send System Exclusive (SysEx) messages to this object.

let kMIDIPropertyDriverDeviceEditorApp: CFString

The full path to an app on the system that configures driver-owned devices.

let kMIDIPropertyNameConfiguration: CFString

An XML representation of the device’s current patch, note, and control name values.

Deprecated

### Presentation

let kMIDIPropertyImage: CFString

The full path to a device icon on the system.

let kMIDIPropertyDisplayName: CFString

The user-visible name for an endpoint that combines the device and endpoint names.

### Audio

let kMIDIPropertyPanDisruptsStereo: CFString

A Boolean value that indicates whether the MIDI pan messages sent to the device or entity cause undesirable effects when playing stereo sounds.

### Protocols

let kMIDIPropertyProtocolID: CFString

The native protocol in which the endpoint communicates.

### Timing

let kMIDIPropertyTransmitsMTC: CFString

A Boolean value that indicates whether the device or entity transmits MIDI Time Code messages.

let kMIDIPropertyReceivesMTC: CFString

A Boolean value that indicates whether the device or entity responds to MIDI Time Code messages.

let kMIDIPropertyTransmitsClock: CFString

A Boolean value that indicates whether the device or entity transmits MIDI beat clock messages.

let kMIDIPropertyReceivesClock: CFString

A Boolean value that indicates whether the device or entity responds to MIDI beat clock messages.

let kMIDIPropertyAdvanceScheduleTimeMuSec: CFString

The recommended number of microseconds in advance that clients should schedule output.

### Roles

let kMIDIPropertyIsMixer: CFString

A Boolean value that indicates whether the device or entity mixes external audio signals.

let kMIDIPropertyIsSampler: CFString

A Boolean value that indicates whether the device or entity plays audio samples in response to MIDI note messages.

let kMIDIPropertyIsEffectUnit: CFString

A Boolean value that indicates whether the device or entity primarily acts as a MIDI-controlled audio effect.

let kMIDIPropertyIsDrumMachine: CFString

A Boolean value that indicates whether the device or entity’s samples aren’t transposable, as with a drum kit.

### Status

let kMIDIPropertyOffline: CFString

A Boolean value that indicates whether the object is offline.

let kMIDIPropertyPrivate: CFString

A Boolean value that indicates whether the system hides an endpoint from other clients.

### Drivers

let kMIDIPropertyDriverOwner: CFString

The name of the driver that owns a device, entity, or endpoint.

let kMIDIPropertyDriverVersion: CFString

The version of the driver that owns a device, entity, or endpoint.

### Connections

let kMIDIPropertyCanRoute: CFString

A Boolean value that indicates whether the device or entity can route messages to or from external MIDI devices.

let kMIDIPropertyIsBroadcast: CFString

A Boolean value that indicates whether the endpoint broadcasts messages to all of the other endpoints in the device.

let kMIDIPropertyConnectionUniqueID: CFString

The unique identifier of an external device attached to this connection.

let kMIDIPropertyIsEmbeddedEntity: CFString

A Boolean value that indicates whether this entity or endpoint has external MIDI connections.

let kMIDIPropertySingleRealtimeEntity: CFString

The 0-based index of the entity on which incoming real-time messages from the device appear to have originated.

### Channels

let kMIDIPropertyReceiveChannels: CFString

The bitmap of channels on which the object receives messages.

let kMIDIPropertyTransmitChannels: CFString

The bitmap of channels on which the object transmits messages.

let kMIDIPropertyMaxReceiveChannels: CFString

The maximum number of MIDI channels on which a device may simultaneously receive channel messages.

let kMIDIPropertyMaxTransmitChannels: CFString

The maximum number of MIDI channels on which a device may simultaneously transmit channel messages.

### Banks

let kMIDIPropertyReceivesBankSelectLSB: CFString

A Boolean value that indicates whether the device or entity responds to MIDI bank select LSB messages.

let kMIDIPropertyReceivesBankSelectMSB: CFString

A Boolean value that indicates whether the device or entity responds to MIDI bank select MSB messages.

let kMIDIPropertyTransmitsBankSelectLSB: CFString

A Boolean value that indicates whether the device or entity transmits MIDI bank select LSB messages.

let kMIDIPropertyTransmitsBankSelectMSB: CFString

A Boolean value that indicates whether the device or entity transmits MIDI bank select MSB messages.

### Notes

let kMIDIPropertyReceivesNotes: CFString

A Boolean value that indicates whether the device or entity responds to MIDI Note On messages.

let kMIDIPropertyTransmitsNotes: CFString

A Boolean value that indicates whether the device or entity transmits MIDI note messages.

### Program Changes

let kMIDIPropertyReceivesProgramChanges: CFString

A Boolean value that indicates whether the device or entity responds to MIDI Program Change messages.

let kMIDIPropertyTransmitsProgramChanges: CFString

A Boolean value that indicates whether the device or entity transmits MIDI Program Change messages.

### Property Accessors

func MIDIObjectGetProperties(MIDIObjectRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFPropertyList>?>, Bool) -> OSStatus

Returns all properties of an object.

func MIDIObjectRemoveProperty(MIDIObjectRef, CFString) -> OSStatus

Removes an object’s property.

func MIDIObjectGetStringProperty(MIDIObjectRef, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Gets an object’s string-type property.

func MIDIObjectSetStringProperty(MIDIObjectRef, CFString, CFString) -> OSStatus

Sets an object’s string-type property.

func MIDIObjectGetIntegerProperty(MIDIObjectRef, CFString, UnsafeMutablePointer&lt;Int32>) -> OSStatus

Gets an object’s integer-type property.

func MIDIObjectSetIntegerProperty(MIDIObjectRef, CFString, Int32) -> OSStatus

Sets an object’s integer-type property.

func MIDIObjectGetDataProperty(MIDIObjectRef, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>) -> OSStatus

Gets an object’s data-type property.

func MIDIObjectSetDataProperty(MIDIObjectRef, CFString, CFData) -> OSStatus

Sets an object’s data-type property.

func MIDIObjectGetDictionaryProperty(MIDIObjectRef, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

Gets an object’s dictionary-type property.

func MIDIObjectSetDictionaryProperty(MIDIObjectRef, CFString, CFDictionary) -> OSStatus

Sets an object’s dictionary-type property.

### Notifications

struct MIDIObjectAddRemoveNotification

A message that describes the addition or removal of an object.

struct MIDIObjectPropertyChangeNotification

A message that describes the change to an object property.

## See Also

### MIDI object configuration

func MIDIObjectFindByUniqueID(MIDIUniqueID, UnsafeMutablePointer&lt;MIDIObjectRef>?, UnsafeMutablePointer&lt;MIDIObjectType>?) -> OSStatus

Locates a device, entity, or endpoint by its unique identifier.

typealias MIDIObjectRef

The common base class for many of the framework’s objects.

