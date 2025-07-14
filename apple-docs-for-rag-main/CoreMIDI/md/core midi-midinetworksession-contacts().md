

- Core MIDI
- MIDINetworkSession
-  contacts() 

Instance Method

# contacts()

Returns the array of network hosts.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func contacts() -> Set
```

## Return Value

The set of MIDI network host objects.

## See Also

### Managing Contacts

func addContact(MIDINetworkHost) -> Bool

Adds a host as a contact.

func removeContact(MIDINetworkHost) -> Bool

Removes a host as a contact.

let MIDINetworkNotificationContactsDidChange: String

Indicates that the list of contacts changed.

