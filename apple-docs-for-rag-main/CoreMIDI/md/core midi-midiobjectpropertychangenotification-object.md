

- Core MIDI
- MIDIObjectPropertyChangeNotification
-  object 

Instance Property

# object

The object whose property changed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var object: MIDIObjectRef
```

## See Also

### Inspecting the Notification

var messageID: MIDINotificationMessageID

The message type.

var messageSize: UInt32

The message size.

var objectType: MIDIObjectType

The object type.

var propertyName: Unmanaged&lt;CFString>

The name of the modified property.

