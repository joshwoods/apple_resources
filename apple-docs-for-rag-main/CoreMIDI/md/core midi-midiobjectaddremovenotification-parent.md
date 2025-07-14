

- Core MIDI
- MIDIObjectAddRemoveNotification
-  parent 

Instance Property

# parent

The parent object of the added or removed child.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var parent: MIDIObjectRef
```

## See Also

### Inspecting the Notification

var messageID: MIDINotificationMessageID

The message type.

var messageSize: UInt32

The message size.

var parentType: MIDIObjectType

The parent object type.

var child: MIDIObjectRef

The added or removed child object.

var childType: MIDIObjectType

The child object type.

