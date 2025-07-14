

- Core MIDI
-  MIDIObjectRef 

Type Alias

# MIDIObjectRef

The common base class for many of the framework’s objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDIObjectRef = UInt32
```

## Discussion

MIDI Objects have properties, and often have an owning object, from which they inherit any properties they don’t define themselves.

Developers may add their own private properties, with names that begin with their company’s inverted domain name, but with underscores instead of dots. For example, `com_apple_APrivateAppleProperty`.

## See Also

### MIDI object configuration

func MIDIObjectFindByUniqueID(MIDIUniqueID, UnsafeMutablePointer&lt;MIDIObjectRef>?, UnsafeMutablePointer&lt;MIDIObjectType>?) -> OSStatus

Locates a device, entity, or endpoint by its unique identifier.

MIDI Object Properties

Configure the properties of MIDI objects.

