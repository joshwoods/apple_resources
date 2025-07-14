

- Open Directory
-  ODRecordRemoveValue(\_:\_:\_:\_:) 

Function

# ODRecordRemoveValue(\_:\_:\_:\_:)

Removes a value from a record’s attribute.

Mac CatalystmacOS 10.6+

``` source
func ODRecordRemoveValue(
    _ record: ODRecordRef!,
    _ attribute: String!,
    _ value: CFTypeRef!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`record`  

The record.

`attribute`  

The attribute.

`value`  

The value to remove.

`error`  

An error reference for error details. Can be `NULL`.

## Return Value

`true` if `inValue` is successfully removed from `inAttribute`; otherwise, `false`.

## Discussion

If `inValue` does not exist, `true` is returned and no error is set.

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

func ODRecordRemoveMember(ODRecordRef!, ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a record as a member from a specified group record.

func ODRecordSetNodeCredentials(ODRecordRef!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets node authentication credentials for a given record.

func ODRecordSetNodeCredentialsExtended(ODRecordRef!, String!, String!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;ODContext>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets node authentication credentials for a record using a specified authentication method.

func ODRecordSetValue(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets one or more attribute values of a record.

func ODRecordSynchronize(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Synchronizes a record with the directory to get current data and commit changes.

