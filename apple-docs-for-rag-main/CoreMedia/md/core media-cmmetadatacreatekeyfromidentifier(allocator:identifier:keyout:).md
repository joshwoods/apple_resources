

- Core Media
-  CMMetadataCreateKeyFromIdentifier(allocator:identifier:keyOut:) 

Function

# CMMetadataCreateKeyFromIdentifier(allocator:identifier:keyOut:)

Creates a copy of the key by using an identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMetadataCreateKeyFromIdentifier(
    allocator: CFAllocator?,
    identifier: CFString,
    keyOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for creating the identifier.

`identifier`  

The identifier to be inspected.

`keyOut`  

Upon return, a pointer to the key data that was used to create the identifier.

## Return Value

If successful, a nonzero result code. See Metadata Identifier Error Codes.

## Discussion

The returned `CFType` is based on the keyspace encoded in the identifier.

For `OSType` keyspaces, the key will be returned as a `CFNumber`, where a big endian interpretation of its CFNumberType.sInt32Type value represents the four bytes of the key’s numeric value.

For the keyspaces kCMMetadataKeySpace_QuickTimeMetadata and kCMMetadataKeySpace_Icy, the key will be returned as a `CFString`.

All other keyspaces will have the function return the key as a `CFData`.

## See Also

### Creating Metadata Identifiers

func CMMetadataCreateIdentifierForKeyAndKeySpace(allocator: CFAllocator?, key: CFTypeRef, keySpace: CFString, identifierOut: UnsafeMutablePointer&lt;CFString?>) -> OSStatus

Creates a URL-like string identifier that represents a key or keyspace tuple.

func CMMetadataCreateKeyFromIdentifierAsCFData(allocator: CFAllocator?, identifier: CFString, keyOut: UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Creates a copy of the key by using an identifier, and results in a core foundation data object.

func CMMetadataCreateKeySpaceFromIdentifier(allocator: CFAllocator?, identifier: CFString, keySpaceOut: UnsafeMutablePointer&lt;CFString?>) -> OSStatus

Creates a copy of the keyspace by using an identifier.

