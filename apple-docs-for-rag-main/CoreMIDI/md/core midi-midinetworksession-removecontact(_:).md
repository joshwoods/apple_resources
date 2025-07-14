

- Core MIDI
- MIDINetworkSession
-  removeContact(\_:) 

Instance Method

# removeContact(\_:)

Removes a host as a contact.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func removeContact(_ contact: MIDINetworkHost) -> Bool
```

## Parameters 

`contact`  

The host to remove.

## Return Value

true if the session successfully removed the host, otherwise false.

## See Also

### Managing Contacts

func contacts() -> Set&lt;MIDINetworkHost>

Returns the array of network hosts.

func addContact(MIDINetworkHost) -> Bool

Adds a host as a contact.

let MIDINetworkNotificationContactsDidChange: String

Indicates that the list of contacts changed.

