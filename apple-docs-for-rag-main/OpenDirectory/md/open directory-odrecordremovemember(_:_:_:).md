

- Open Directory
-  ODRecordRemoveMember(\_:\_:\_:) 

Function

# ODRecordRemoveMember(\_:\_:\_:)

Removes a record as a member from a specified group record.

Mac CatalystmacOS 10.6+

``` source
func ODRecordRemoveMember(
    _ group: ODRecordRef!,
    _ member: ODRecordRef!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`group`  

The group record.

`member`  

The record to remove.

`error`  

An error reference for error details. Can be `NULL`.

## Return Value

`true` if `inMember` is successfully removed from `inGroup`; otherwise, `false`.

## See Also

### Working with Records

func ODRecordAddMember(ODRecordRef!, ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Adds a record as a member of a group record.

func ODRecordAddValue(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Adds a value to an attribute of a record.

func ODRecordChangePassword(ODRecordRef!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Changes the password of a record.

func ODRecordContainsMember(ODRecordRef!, ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns whether a group record contains a given record.

func ODRecordCopyDetails(ODRecordRef!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

Returns the values of a record’s attributes.

func ODRecordCopyValues(ODRecordRef!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns the value of a single attribute of a record.

func ODRecordDelete(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Deletes a record from a node and invalidates the record.

func ODRecordGetRecordName(ODRecordRef!) -> Unmanaged&lt;CFString>!

Returns the official name of a record.

func ODRecordGetRecordType(ODRecordRef!) -> Unmanaged&lt;CFString>!

Returns the type of a record.

func ODRecordGetTypeID() -> CFTypeID

Returns the type ID for a record.

func ODRecordRemoveValue(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a value from a record’s attribute.

func ODRecordSetNodeCredentials(ODRecordRef!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets node authentication credentials for a given record.

func ODRecordSetNodeCredentialsExtended(ODRecordRef!, String!, String!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;ODContext>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets node authentication credentials for a record using a specified authentication method.

func ODRecordSetValue(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets one or more attribute values of a record.

func ODRecordSynchronize(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Synchronizes a record with the directory to get current data and commit changes.

