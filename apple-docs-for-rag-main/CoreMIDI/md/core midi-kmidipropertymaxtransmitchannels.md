

- Core MIDI
-  kMIDIPropertyMaxTransmitChannels 

Global Variable

# kMIDIPropertyMaxTransmitChannels

The maximum number of MIDI channels on which a device may simultaneously transmit channel messages.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
let kMIDIPropertyMaxTransmitChannels: CFString
```

## Discussion

Common values are 0, 1, and 16.

## See Also

### Channels

let kMIDIPropertyReceiveChannels: CFString

The bitmap of channels on which the object receives messages.

let kMIDIPropertyTransmitChannels: CFString

The bitmap of channels on which the object transmits messages.

let kMIDIPropertyMaxReceiveChannels: CFString

The maximum number of MIDI channels on which a device may simultaneously receive channel messages.

