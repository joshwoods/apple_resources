

- Core MIDI
- MIDINetworkSession
-  addContact(\_:) 

Instance Method

# addContact(\_:)

Adds a host as a contact.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func addContact(_ contact: MIDINetworkHost) -> Bool
```

## Parameters 

`contact`  

The MIDI network host to add.

## Return Value

true if the session successfully added the host, otherwise false.

## See Also

### Managing Contacts

func contacts() -> Set&lt;MIDINetworkHost>

Returns the array of network hosts.

func removeContact(MIDINetworkHost) -> Bool

Removes a host as a contact.

let MIDINetworkNotificationContactsDidChange: String

Indicates that the list of contacts changed.

