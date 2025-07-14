

- Core MIDI
-  MIDIObjectPropertyChangeNotification 

Structure

# MIDIObjectPropertyChangeNotification

A message that describes the change to an object property.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIObjectPropertyChangeNotification
```

## Topics

### Inspecting the Notification

var messageID: MIDINotificationMessageID

The message type.

var messageSize: UInt32

The message size.

var object: MIDIObjectRef

The object whose property changed.

var objectType: MIDIObjectType

The object type.

var propertyName: Unmanaged&lt;CFString>

The name of the modified property.

### Initializers

init(messageID: MIDINotificationMessageID, messageSize: UInt32, object: MIDIObjectRef, objectType: MIDIObjectType, propertyName: Unmanaged&lt;CFString>)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Notifications

struct MIDIObjectAddRemoveNotification

A message that describes the addition or removal of an object.

