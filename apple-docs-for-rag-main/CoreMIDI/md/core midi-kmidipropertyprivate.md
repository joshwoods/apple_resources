

- Core MIDI
-  kMIDIPropertyPrivate 

Global Variable

# kMIDIPropertyPrivate

A Boolean value that indicates whether the system hides an endpoint from other clients.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
let kMIDIPropertyPrivate: CFString
```

## Discussion

You can set this property on a device or entity, but it still appears in the API; the system only hides the object’s owned endpoints.

## See Also

### Status

let kMIDIPropertyOffline: CFString

A Boolean value that indicates whether the object is offline.

