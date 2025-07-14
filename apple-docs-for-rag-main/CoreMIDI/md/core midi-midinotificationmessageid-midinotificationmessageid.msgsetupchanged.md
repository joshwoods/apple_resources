

- Core MIDI
- MIDINotificationMessageID
-  MIDINotificationMessageID.msgSetupChanged 

Case

# MIDINotificationMessageID.msgSetupChanged

Some aspect of the current MIDI setup changed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case msgSetupChanged
```

## Discussion

This type provides no data. Ignore this message if you’re explicitly handling other state changes.

## See Also

### Change Types

case msgObjectAdded

The system added a device, entity, or endpoint.

case msgObjectRemoved

The system removed a device, entity, or endpoint.

case msgPropertyChanged

An object’s property value changed.

case msgThruConnectionsChanged

The system created or disposed of a persistent MIDI Thru connection.

case msgSerialPortOwnerChanged

The system changed a serial port owner.

case msgIOError

A driver I/O error occurred.

