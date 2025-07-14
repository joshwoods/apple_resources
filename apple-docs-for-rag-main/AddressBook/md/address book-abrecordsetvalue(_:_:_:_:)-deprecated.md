

- Address Book
-  ABRecordSetValue(\_:\_:\_:\_:) Deprecated

Function

# ABRecordSetValue(\_:\_:\_:\_:)

Sets the value of a given property for a record.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS

**iOS, iPadOS, Mac Catalyst**

``` source
func ABRecordSetValue(
    _ record: ABRecord!,
    _ property: ABPropertyID,
    _ value: CFTypeRef!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

**macOS**

``` source
func ABRecordSetValue(
    _ record: ABRecordRef!,
    _ property: CFString!,
    _ value: CFTypeRef!
) -> Bool
```

Deprecated

use CN mutable object's properties

## Parameters 

`record`  

The record you wish to modify.

`property`  

The property whose value you wish to set. May be a pre-defined or program-defined property. See `Common Properties` for a list of properties all records have, and specific ABRecord derived opaque types for any additional properties. If `NULL`, this function raises an exception.

`value`  

The new value for `property` in `record`. If `NULL` or not the correct type, this function raises an exception.

## Return Value

If `property` isa multi-value list property, this method checks to see if the valuesin the multi-value list are the same type. If the multi-value list containsmixed types, this method returns `false`.Returns `true` if successful, `false` otherwise.

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

func ABRemoveRecord(ABAddressBookRef!, ABRecordRef!) -> Bool

Removes the specified record from the Address Book database.

