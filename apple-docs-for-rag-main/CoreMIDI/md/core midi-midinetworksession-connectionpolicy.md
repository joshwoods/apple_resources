

- Core MIDI
- MIDINetworkSession
-  connectionPolicy 

Instance Property

# connectionPolicy

The policy that determines who can connect to this session.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var connectionPolicy: MIDINetworkConnectionPolicy { get set }
```

## Topics

### Connection Policies

enum MIDINetworkConnectionPolicy

## See Also

### Configuring a Session

class func `default`() -> MIDINetworkSession

Returns the default singleton session.

var isEnabled: Bool

A Boolean value that determines whether the session is enabled.

