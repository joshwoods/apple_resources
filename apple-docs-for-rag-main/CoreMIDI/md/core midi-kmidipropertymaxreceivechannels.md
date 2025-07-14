

- Core MIDI
-  kMIDIPropertyMaxReceiveChannels 

Global Variable

# kMIDIPropertyMaxReceiveChannels

The maximum number of MIDI channels on which a device may simultaneously receive channel messages.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
let kMIDIPropertyMaxReceiveChannels: CFString
```

## Discussion

The property value ranges from 0 to 16. Values for this property indicate:

- 0 for devices that only respond to system messages

- 1 for nonmultitimbral devices

- 2 to 15 for multitimbral devices with fewer than 16 voices

- 16 for fully multitimbral devices

## See Also

### Channels

let kMIDIPropertyReceiveChannels: CFString

The bitmap of channels on which the object receives messages.

let kMIDIPropertyTransmitChannels: CFString

The bitmap of channels on which the object transmits messages.

let kMIDIPropertyMaxTransmitChannels: CFString

The maximum number of MIDI channels on which a device may simultaneously transmit channel messages.

