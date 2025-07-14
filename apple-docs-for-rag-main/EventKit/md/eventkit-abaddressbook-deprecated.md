

- EventKit
-  ABAddressBook Deprecated

Type Alias

# ABAddressBook

A reference to an ABAddressBook object.

visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
typealias ABAddressBook = CFTypeRef
```

Deprecated

use CNContactStore

## See Also

### Finding Participant Address Book Records

func abRecord(with: ABAddressBook) -> ABRecord?

Returns the address book record that represents the participant.

func abPerson(in: ABAddressBook) -> ABPerson?

Returns the address book record that represents the participant.

Deprecated

typealias ABRecord

A reference to an ABRecord object or any of its derivedopaque types.

Deprecated

