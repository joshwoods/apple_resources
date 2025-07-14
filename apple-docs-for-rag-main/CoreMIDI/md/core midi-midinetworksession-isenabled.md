

- Core MIDI
- MIDINetworkSession
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that determines whether the session is enabled.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

The default value is false. Disabled sessions don’t appear on the network and can’t initiate or receive connections.

## See Also

### Configuring a Session

class func `default`() -> MIDINetworkSession

Returns the default singleton session.

var connectionPolicy: MIDINetworkConnectionPolicy

The policy that determines who can connect to this session.

