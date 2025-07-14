

- Address Book
-  ABMultiValueInsertValueAndLabelAtIndex(\_:\_:\_:\_:\_:) Deprecated

Function

# ABMultiValueInsertValueAndLabelAtIndex(\_:\_:\_:\_:\_:)

Inserts a value and a label into a multivalue property.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func ABMultiValueInsertValueAndLabelAtIndex(
    _ multiValue: ABMutableMultiValue!,
    _ value: CFTypeRef!,
    _ label: CFString!,
    _ index: CFIndex,
    _ outIdentifier: UnsafeMutablePointer!
) -> Bool
```

Deprecated

use \[NSMutableArray insertObject:\[CNLabeledValue labeledValueWithLabel:value:\] atIndex:\]

## Parameters 

`multiValue`  

The multivalue property into which to insert `value`.

`value`  

The value to insert.

`label`  

The label to insert.

`index`  

The location, in `multiValue`, at which to insert `value` and `label`.

Raises an exception when out of bounds.

`outIdentifier`  

On output, the identifier of the added value.

## Return Value

`true` when value and label are inserted successfully into multiValue, `false` otherwise.

## Discussion

This function performs no type checking. It allows the insertion of values whose type does not match the type declared for `multiValue`.

This function takes an index. If you have an identifier, use the ABMultiValueGetIndexForIdentifier(_:_:) function to get the corresponding index.

## See Also

### Deprecated

func ABAddressBookAddRecord(ABAddressBook!, ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Adds a record to an address book.

Deprecated

func ABAddressBookCopyArrayOfAllGroups(ABAddressBook!) -> Unmanaged&lt;CFArray>!

Returns an array with all the groups in an address book.

Deprecated

func ABAddressBookCopyArrayOfAllGroupsInSource(ABAddressBook!, ABRecord!) -> Unmanaged&lt;CFArray>!

Returns an array of all groups from a particular source.

Deprecated

func ABAddressBookCopyArrayOfAllPeople(ABAddressBook!) -> Unmanaged&lt;CFArray>!

Returns all the person records in an address book.

Deprecated

func ABAddressBookCopyArrayOfAllPeopleInSource(ABAddressBook!, ABRecord!) -> Unmanaged&lt;CFArray>!

Returns an array of all person records from a particular source.

Deprecated

func ABAddressBookCopyArrayOfAllPeopleInSourceWithSortOrdering(ABAddressBook!, ABRecord!, ABPersonSortOrdering) -> Unmanaged&lt;CFArray>!

Returns an array of all person records in the address book, sorted with the specified order.

Deprecated

func ABAddressBookCopyArrayOfAllSources(ABAddressBook!) -> Unmanaged&lt;CFArray>!

Returns an array of all sources in the address book.

Deprecated

func ABAddressBookCopyDefaultSource(ABAddressBook!) -> Unmanaged&lt;ABRecord>!

Returns the default source.

Deprecated

func ABAddressBookCopyLocalizedLabel(CFString!) -> Unmanaged&lt;CFString>!

Returns a localized version of a record-property label.

Deprecated

func ABAddressBookCopyPeopleWithName(ABAddressBook!, CFString!) -> Unmanaged&lt;CFArray>!

Performs a prefix search on the composite names of people in an address book and returns an array of persons that match the search criteria.

Deprecated

func ABAddressBookCreate() -> Unmanaged&lt;ABAddressBook>!

Creates a new address book object with data from the Address Book database.

Deprecated

func ABAddressBookCreateWithOptions(CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ABAddressBook>!

Creates a new address book object with data from the Address Book database.

Deprecated

func ABAddressBookGetAuthorizationStatus() -> ABAuthorizationStatus

Returns the authorization status of your app for accessing address book data.

Deprecated

func ABAddressBookGetGroupCount(ABAddressBook!) -> CFIndex

Returns the number of groups in an address book.

Deprecated

func ABAddressBookGetGroupWithRecordID(ABAddressBook!, ABRecordID) -> Unmanaged&lt;ABRecord>!

Returns the group with a given record ID.

Deprecated

