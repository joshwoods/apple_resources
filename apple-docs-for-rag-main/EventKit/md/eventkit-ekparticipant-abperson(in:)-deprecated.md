

- EventKit
- EKParticipant
-  abPerson(in:) Deprecated

Instance Method

# abPerson(in:)

Returns the address book record that represents the participant.

macOS 10.8–10.11Deprecated

``` source
func abPerson(in addressBook: ABAddressBook) -> ABPerson?
```

Deprecated

Use contactPredicate instead

## Parameters 

`addressBook`  

The address book to search.

## Return Value

The address book record for the participant, or `nil` if the record is not found.

## Discussion

This method searches for a record match based on the participant’s email address.

### Special Considerations

Note

This instance method is only available in macOS. For iOS, see the abRecord(with:) instance method.

## See Also

### Finding Participant Address Book Records

func abRecord(with: ABAddressBook) -> ABRecord?

Returns the address book record that represents the participant.

typealias ABAddressBook

A reference to an ABAddressBook object.

Deprecated

typealias ABRecord

A reference to an ABRecord object or any of its derivedopaque types.

Deprecated

