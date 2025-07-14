

- EventKit
- EKParticipant
-  abRecord(with:) 

Instance Method

# abRecord(with:)

Returns the address book record that represents the participant.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+

``` source
func abRecord(with addressBook: ABAddressBook) -> ABRecord?
```

## Parameters 

`addressBook`  

The address book to search.

## Return Value

The address book record for the participant, or `nil` if the record is not found.

## Discussion

This method searches for a record match based on the participant’s email address.

### Special Considerations

Note

This instance method is only available on iOS. For macOS, see the abPerson(in:) instance method.

## See Also

### Finding Participant Address Book Records

func abPerson(in: ABAddressBook) -> ABPerson?

Returns the address book record that represents the participant.

Deprecated

typealias ABAddressBook

A reference to an ABAddressBook object.

Deprecated

typealias ABRecord

A reference to an ABRecord object or any of its derivedopaque types.

Deprecated

