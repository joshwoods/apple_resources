

- Address Book
-  ABAddressBookCreateWithOptions(\_:\_:) Deprecated

Function

# ABAddressBookCreateWithOptions(\_:\_:)

Creates a new address book object with data from the Address Book database.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func ABAddressBookCreateWithOptions(
    _ options: CFDictionary!,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

Deprecated

use \[\[CNContactStore alloc\] init\]

## Parameters 

`options`  

Reserved. Pass `NULL`.

`error`  

On error, contains error information. See Address Book Errors.

## Return Value

An address book object, `NULL`, or an empty database.

## Discussion

Changes made to the returned address book are reflected in the Address Book database only after saving the address book with ABAddressBookSave(_:_:).

On iOS 6.0 and later, if the caller does not have access to the Address Book database:

- For apps linked against iOS 6.0 and later, this function returns `NULL`.

- For apps linked against previous version of iOS, this function returns an empty read-only database.

If your app syncs information with the database, it must not sync data when it does not have access to the database.

Important

You must ensure that an instance of `ABAddressBookRef` is used by only one thread.

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

func ABAddressBookGetAuthorizationStatus() -> ABAuthorizationStatus

Returns the authorization status of your app for accessing address book data.

Deprecated

func ABAddressBookGetGroupCount(ABAddressBook!) -> CFIndex

Returns the number of groups in an address book.

Deprecated

func ABAddressBookGetGroupWithRecordID(ABAddressBook!, ABRecordID) -> Unmanaged&lt;ABRecord>!

Returns the group with a given record ID.

Deprecated

func ABAddressBookGetPersonCount(ABAddressBook!) -> CFIndex

Returns the number of person records in an address book.

Deprecated

