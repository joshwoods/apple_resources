

- Address Book
-  ABRemoveRecord(\_:\_:) 

Function

# ABRemoveRecord(\_:\_:)

Removes the specified record from the Address Book database.

macOS

``` source
func ABRemoveRecord(
    _ addressBook: ABAddressBookRef!,
    _ record: ABRecordRef!
) -> Bool
```

## Parameters 

`addressBook`  

The address book for the logged-in user.

`record`  

The ABRecord object to be removed. If `NULL`, this function raises an exception.

## Return Value

`true` if the record was removed successfully, `false` otherwise.

## See Also

### Records

func ABAddRecord(ABAddressBookRef!, ABRecordRef!) -> Bool

Adds a record of the specified type to the Address Book database.

func ABCopyRecordForUniqueId(ABAddressBookRef!, CFString!) -> Unmanaged&lt;ABRecordRef>!

Returns the record that matches the given unique ID.

func ABCopyRecordTypeFromUniqueId(ABAddressBookRef!, CFString!) -> Unmanaged&lt;CFString>!

Returns the type name of the record that matches a given unique ID.

func ABCreateFormattedAddressFromDictionary(ABAddressBookRef!, CFDictionary!) -> Unmanaged&lt;CFString>!

Returns a string containing the formatted address.

func ABRecordCopyRecordType(ABRecordRef!) -> Unmanaged&lt;CFString>!

Returns the type of the given record.

func ABRecordCopyUniqueId(ABRecordRef!) -> Unmanaged&lt;CFString>!

Returns the unique ID of the receiver.

func ABRecordCopyValue(ABRecord!, ABPropertyID) -> Unmanaged&lt;CFTypeRef>!

Returns the value of the given property.

Deprecated

func ABRecordCreateCopy(ABRecordRef!) -> Unmanaged&lt;ABRecordRef>!

Returns a copy of the given record.

func ABRecordIsReadOnly(ABRecordRef!) -> Bool

Returns whether or not the record is read-only.

func ABRecordRemoveValue(ABRecord!, ABPropertyID, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes the value of the given property.

Deprecated

func ABRecordSetValue(ABRecord!, ABPropertyID, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the value of a given property for a record.

Deprecated

