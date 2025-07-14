

- Address Book
-  ABRecordCreateCopy(\_:) 

Function

# ABRecordCreateCopy(\_:)

Returns a copy of the given record.

macOS 10.4+

``` source
func ABRecordCreateCopy(_ record: ABRecordRef!) -> Unmanaged!
```

## Parameters 

`record`  

The record you wish to copy.

## Return Value

A copy of the specifiedABRecordRef.

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

func ABRecordIsReadOnly(ABRecordRef!) -> Bool

Returns whether or not the record is read-only.

func ABRecordRemoveValue(ABRecord!, ABPropertyID, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes the value of the given property.

Deprecated

func ABRecordSetValue(ABRecord!, ABPropertyID, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the value of a given property for a record.

Deprecated

func ABRemoveRecord(ABAddressBookRef!, ABRecordRef!) -> Bool

Removes the specified record from the Address Book database.

