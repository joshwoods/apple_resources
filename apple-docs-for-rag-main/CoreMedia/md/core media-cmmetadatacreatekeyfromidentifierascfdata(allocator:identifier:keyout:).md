

- Core Media
-  CMMetadataCreateKeyFromIdentifierAsCFData(allocator:identifier:keyOut:) 

Function

# CMMetadataCreateKeyFromIdentifierAsCFData(allocator:identifier:keyOut:)

Creates a copy of the key by using an identifier, and results in a core foundation data object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMetadataCreateKeyFromIdentifierAsCFData(
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

The bytes in the `CFData` correspond to how they are serialized in the file.

## See Also

### Creating Metadata Identifiers

func CMMetadataCreateIdentifierForKeyAndKeySpace(allocator: CFAllocator?, key: CFTypeRef, keySpace: CFString, identifierOut: UnsafeMutablePointer&lt;CFString?>) -> OSStatus

Creates a URL-like string identifier that represents a key or keyspace tuple.

func CMMetadataCreateKeyFromIdentifier(allocator: CFAllocator?, identifier: CFString, keyOut: UnsafeMutablePointer&lt;CFTypeRef?>) -> OSStatus

Creates a copy of the key by using an identifier.

func CMMetadataCreateKeySpaceFromIdentifier(allocator: CFAllocator?, identifier: CFString, keySpaceOut: UnsafeMutablePointer&lt;CFString?>) -> OSStatus

Creates a copy of the keyspace by using an identifier.

