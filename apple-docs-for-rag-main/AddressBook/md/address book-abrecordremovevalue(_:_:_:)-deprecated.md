

- Address Book
-  ABRecordRemoveValue(\_:\_:\_:) Deprecated

Function

# ABRecordRemoveValue(\_:\_:\_:)

Removes the value of the given property.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS

**macOS**

``` source
func ABRecordRemoveValue(
    _ record: ABRecordRef!,
    _ property: CFString!
) -> Bool
```

**iOS, iPadOS, Mac Catalyst**

``` source
func ABRecordRemoveValue(
    _ record: ABRecord!,
    _ property: ABPropertyID,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

Deprecated

use CN mutable object's properties, setting to @, @\[\], or nil

## Parameters 

`record`  

The record whose value you wish to remove.

`property`  

The property name in `record` whose value you wish to remove. May be a pre-defined or program-defined property. See `Common Properties` for a list of properties all records have, and specific ABRecord derived opaque types for any additional properties.

## Return Value

The value for `property` in `record`.The type of the returned value depends on the property type (see PropertyTypes for a list of possible property types). You are responsiblefor releasing this object.

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

func ABRecordSetValue(ABRecord!, ABPropertyID, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the value of a given property for a record.

Deprecated

func ABRemoveRecord(ABAddressBookRef!, ABRecordRef!) -> Bool

Removes the specified record from the Address Book database.

