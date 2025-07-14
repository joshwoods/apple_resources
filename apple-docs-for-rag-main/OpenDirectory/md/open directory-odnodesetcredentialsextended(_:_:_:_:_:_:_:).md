

- Open Directory
-  ODNodeSetCredentialsExtended(\_:\_:\_:\_:\_:\_:\_:) 

Function

# ODNodeSetCredentialsExtended(\_:\_:\_:\_:\_:\_:\_:)

Sets credentials for interacting with a node using a specified authentication method.

Mac CatalystmacOS 10.6+

``` source
func ODNodeSetCredentialsExtended(
    _ node: ODNodeRef!,
    _ recordType: String!,
    _ authType: String!,
    _ authItems: CFArray!,
    _ outAuthItems: UnsafeMutablePointer?>!,
    _ outContext: UnsafeMutablePointer?>!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`node`  

The node.

`recordType`  

The record type that uses the credentials. Can be `NULL`. The default value is `kODRecordTypeUsers`.

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

`true` if no error occurs; otherwise, `false`.

## Discussion

If this function fails, the previous credentials for the node are used.

This function sets credentials for all references to the node. If you only want to set credentials for a single record referencing the node, use ODRecordSetNodeCredentialsExtended(_:_:_:_:_:_:_:) instead.

## See Also

### Related Documentation

Record Types

Types of Open Directory records.

Authentication Types

Types of authentication available in Open Directory.

### Working with Nodes

func ODNodeCopyDetails(ODNodeRef!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

Returns a dictionary containing details about a node.

func ODNodeCopyRecord(ODNodeRef!, String!, CFString!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODRecordRef>!

Returns a reference to a record of a node.

func ODNodeCopySubnodeNames(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns the names of subnodes for a given node.

func ODNodeCopySupportedAttributes(ODNodeRef!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns an array of attribute types supported by a given node.

func ODNodeCopySupportedRecordTypes(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns an array of the record types supported by a given node.

func ODNodeCopyUnreachableSubnodeNames(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns an array of the subnodes of a given node that are currently unreachable.

func ODNodeCreateCopy(CFAllocator!, ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODNodeRef>!

Returns a copy of an existing node.

func ODNodeCreateRecord(ODNodeRef!, String!, CFString!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODRecordRef>!

Creates a record in a specified node with specified properties.

func ODNodeCreateWithName(CFAllocator!, ODSessionRef!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODNodeRef>!

Returns a new node created with a specified name.

func ODNodeCreateWithNodeType(CFAllocator!, ODSessionRef!, ODNodeType, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODNodeRef>!

Returns a new node created with a specified type.

func ODNodeCustomCall(ODNodeRef!, CFIndex, CFData!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFData!

Returns the result of a custom call to a node.

func ODNodeGetName(ODNodeRef!) -> Unmanaged&lt;CFString>!

Returns the name of a node.

func ODNodeGetTypeID() -> CFTypeID

Returns the type ID for an Open Directory node.

func ODNodeSetCredentials(ODNodeRef!, String!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets credentials for interacting with a node.

