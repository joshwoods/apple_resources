

- Core MIDI
-  kMIDIPropertyReceiveChannels 

Global Variable

# kMIDIPropertyReceiveChannels

The bitmap of channels on which the object receives messages.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
let kMIDIPropertyReceiveChannels: CFString
```

## Discussion

You can use this property in the following scenarios:

- Drivers can set this property on their entities and endpoints.

- Studio setup editors can allow the user to set this property on external endpoints.

- Virtual destinations can set this property on their endpoints.

## See Also

### Channels

let kMIDIPropertyTransmitChannels: CFString

The bitmap of channels on which the object transmits messages.

let kMIDIPropertyMaxReceiveChannels: CFString

The maximum number of MIDI channels on which a device may simultaneously receive channel messages.

let kMIDIPropertyMaxTransmitChannels: CFString

The maximum number of MIDI channels on which a device may simultaneously transmit channel messages.

