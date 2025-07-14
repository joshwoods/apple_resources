

- Core MIDI
- MIDINotificationMessageID
-  MIDINotificationMessageID.msgObjectRemoved 

Case

# MIDINotificationMessageID.msgObjectRemoved

The system removed a device, entity, or endpoint.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case msgObjectRemoved
```

## Discussion

This type’s data is MIDIObjectAddRemoveNotification.

## See Also

### Change Types

case msgSetupChanged

Some aspect of the current MIDI setup changed.

case msgObjectAdded

The system added a device, entity, or endpoint.

case msgPropertyChanged

An object’s property value changed.

case msgThruConnectionsChanged

The system created or disposed of a persistent MIDI Thru connection.

case msgSerialPortOwnerChanged

The system changed a serial port owner.

case msgIOError

A driver I/O error occurred.

