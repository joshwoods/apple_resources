

- Core MIDI
- MIDINetworkSession
-  default() 

Type Method

# default()

Returns the default singleton session.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class func `default`() -> MIDINetworkSession
```

## Return Value

The default session.

## See Also

### Configuring a Session

var isEnabled: Bool

A Boolean value that determines whether the session is enabled.

var connectionPolicy: MIDINetworkConnectionPolicy

The policy that determines who can connect to this session.

