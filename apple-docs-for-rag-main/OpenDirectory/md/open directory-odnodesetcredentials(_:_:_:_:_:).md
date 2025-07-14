

- Open Directory
-  ODNodeSetCredentials(\_:\_:\_:\_:\_:) 

Function

# ODNodeSetCredentials(\_:\_:\_:\_:\_:)

Sets credentials for interacting with a node.

Mac CatalystmacOS 10.6+

``` source
func ODNodeSetCredentials(
    _ node: ODNodeRef!,
    _ recordType: String!,
    _ recordName: CFString!,
    _ password: CFString!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`node`  

The node.

`recordType`  

The record type that uses the credentials. Can be `NULL`. The default value is `kODRecordTypeUsers`.

`recordName`  

The username to use to authenticate with the node.

`password`  

The password to use to authenticate with the node.

`error`  

An error reference for error details. Can be `NULL`.

## Return Value

`true` if the credentials are successfully set; otherwise, `false`.

## Discussion

If this function fails, the previous credentials for the node are used.

This function sets credentials for all references to the node. If you only want to set credentials for a single record referencing the node, use ODRecordSetNodeCredentials(_:_:_:_:) instead.

## See Also

### Related Documentation

Record Types

Types of Open Directory records.

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

func ODNodeSetCredentialsExtended(ODNodeRef!, String!, String!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;ODContext>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets credentials for interacting with a node using a specified authentication method.

