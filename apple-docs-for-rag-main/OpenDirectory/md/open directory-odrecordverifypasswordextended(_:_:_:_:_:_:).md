

- Open Directory
-  ODRecordVerifyPasswordExtended(\_:\_:\_:\_:\_:\_:) 

Function

# ODRecordVerifyPasswordExtended(\_:\_:\_:\_:\_:\_:)

Verifies a given password for a record given a specified authentication method.

Mac CatalystmacOS 10.6+

``` source
func ODRecordVerifyPasswordExtended(
    _ record: ODRecordRef!,
    _ authType: String!,
    _ authItems: CFArray!,
    _ outAuthItems: UnsafeMutablePointer?>!,
    _ outContext: UnsafeMutablePointer?>!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`record`  

The record.

`authType`  

The type of authentication to use.

`authItems`  

An array of `CFString` or `CFData` objects to be used in the authentication process.

`outAuthItems`  

An array of `CFData` objects returned from the authentication process, if any are returned; `NULL` otherwise.

`outContext`  

The proper context if the authentication attempt requires a context; `NULL` otherwise. If not `NULL`, then more calls must be made with the Context to continue the authentication.

`error`  

An error reference for error details. Can be `NULL`.

## Return Value

`true` if the authentication information is valid; otherwise, `false`.

## See Also

### Related Documentation

Authentication Types

Types of authentication available in Open Directory.

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

func ODRecordRemoveValue(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a value from a record’s attribute.

func ODRecordSetNodeCredentials(ODRecordRef!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets node authentication credentials for a given record.

func ODRecordSetNodeCredentialsExtended(ODRecordRef!, String!, String!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;ODContext>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets node authentication credentials for a record using a specified authentication method.

func ODRecordSetValue(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets one or more attribute values of a record.

