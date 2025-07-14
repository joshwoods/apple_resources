

- Core MIDI
-  MIDIObjectAddRemoveNotification 

Structure

# MIDIObjectAddRemoveNotification

A message that describes the addition or removal of an object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIObjectAddRemoveNotification
```

## Topics

### Inspecting the Notification

var messageID: MIDINotificationMessageID

The message type.

var messageSize: UInt32

The message size.

var parent: MIDIObjectRef

The parent object of the added or removed child.

var parentType: MIDIObjectType

The parent object type.

var child: MIDIObjectRef

The added or removed child object.

var childType: MIDIObjectType

The child object type.

### Initializers

init()

init(messageID: MIDINotificationMessageID, messageSize: UInt32, parent: MIDIObjectRef, parentType: MIDIObjectType, child: MIDIObjectRef, childType: MIDIObjectType)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Notifications

struct MIDIObjectPropertyChangeNotification

A message that describes the change to an object property.

