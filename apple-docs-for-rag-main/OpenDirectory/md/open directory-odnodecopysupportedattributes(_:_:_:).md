

- Open Directory
-  ODNodeCopySupportedAttributes(\_:\_:\_:) 

Function

# ODNodeCopySupportedAttributes(\_:\_:\_:)

Returns an array of attribute types supported by a given node.

Mac CatalystmacOS 10.6+

``` source
func ODNodeCopySupportedAttributes(
    _ node: ODNodeRef!,
    _ recordType: String!,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`node`  

The node.

`recordType`  

The record type to list supported attribute types for. Can be `NULL`.

`error`  

An error reference for error details. Can be `NULL`.

## Return Value

An array of supported attribute types.

## Discussion

If `inRecordType` is `NULL`, this function returns all attribute types supported by all record types of the node; otherwise, only attribute types specific to `inRecordType` are returned.

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

func ODNodeSetCredentialsExtended(ODNodeRef!, String!, String!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;ODContext>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets credentials for interacting with a node using a specified authentication method.

