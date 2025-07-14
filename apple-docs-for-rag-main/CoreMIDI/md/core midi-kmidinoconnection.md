

- Core MIDI
-  kMIDINoConnection 

Global Variable

# kMIDINoConnection

The connection you’re trying to close doesn’t exist.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kMIDINoConnection: OSStatus { get }
```

## See Also

### Error Codes

var kMIDIInvalidClient: OSStatus

The client is invalid.

var kMIDIInvalidPort: OSStatus

The port is invalid.

var kMIDIWrongEndpointType: OSStatus

A function received a source endpoint when it required a destination endpoint, or vice versa.

var kMIDIUnknownEndpoint: OSStatus

The system doesn’t recognize the endpoint.

var kMIDIUnknownProperty: OSStatus

The property you’re trying to query isn’t set on the object.

var kMIDIWrongPropertyType: OSStatus

The value you assigned to the property is the wrong type.

var kMIDINoCurrentSetup: OSStatus

A MIDI setup object doesn’t currently exist.

var kMIDIMessageSendErr: OSStatus

The communication with the MIDI server failed.

var kMIDIServerStartErr: OSStatus

The system can’t start the MIDI server.

var kMIDISetupFormatErr: OSStatus

The system can’t read the saved state.

var kMIDIWrongThread: OSStatus

A driver is calling a non-I/O function in the server from a thread other than the server’s main thread.

var kMIDIObjectNotFound: OSStatus

The requested object doesn’t exist.

var kMIDIIDNotUnique: OSStatus

The identifier you’re trying to set isn’t unique.

var kMIDINotPermitted: OSStatus

The process doesn’t have privileges for the requested operation.

var kMIDIUnknownError: OSStatus

The system can’t perform the requested operation.

