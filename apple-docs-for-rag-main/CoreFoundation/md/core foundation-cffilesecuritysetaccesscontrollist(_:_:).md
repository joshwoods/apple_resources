

- Core Foundation
-  CFFileSecuritySetAccessControlList(\_:\_:) 

Function

# CFFileSecuritySetAccessControlList(\_:\_:)

Sets the access control list associated with a `CFFileSecurityRef` object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileSecuritySetAccessControlList(
    _ fileSec: CFFileSecurity!,
    _ accessControlList: acl_t!
) -> Bool
```

## Parameters 

`fileSec`  

The `CFFileSecurityRef` object to modify.

`accessControlList`  

The access control list to set, or `kCFFileSecurityRemoveACL` to indicate that the access control list should be removed from a file, or `NULL` to unset the access control list property in the object.

## Return Value

Returns `true` if the access control list was successfully set, or `false` otherwise.

## Discussion

To remove the access control list from a file system object, pass `kCFFileSecurityRemoveACL` as the `accessControlList` parameter. Then, call CFURLSetResourcePropertyForKey(_:_:_:_:) to set kCFURLFileSecurityKey to the resulting `fileSec` object.

Setting the `accessControlList` to `NULL` unsets the ACL property of the `CFFileSecurityRef` object. By doing this, the access control list of the file will be unchanged if you subsequently use this object to set permissions on an actual file system object.

## See Also

### Functions

func CFAllocatorAllocateBytes(CFAllocator!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

func CFAllocatorAllocateTyped(CFAllocator!, CFIndex, CFAllocatorTypeID, CFOptionFlags) -> UnsafeMutableRawPointer!

func CFAllocatorReallocateBytes(CFAllocator!, UnsafeMutableRawPointer!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

func CFAllocatorReallocateTyped(CFAllocator!, UnsafeMutableRawPointer!, CFIndex, CFAllocatorTypeID, CFOptionFlags) -> UnsafeMutableRawPointer!

func CFAttributedStringGetBidiLevelsAndResolvedDirections(CFAttributedString!, CFRange, Int8, UnsafeMutablePointer&lt;UInt8>!, UnsafeMutablePointer&lt;UInt8>!) -> Bool

func CFBundleCopyLocalizedStringForLocalizations(CFBundle!, CFString!, CFString!, CFString!, CFArray!) -> CFString!

Returns a localized string from a bundle’s strings file.

func CFBundleIsArchitectureLoadable(cpu_type_t) -> Bool

func CFBundleIsExecutableLoadable(CFBundle!) -> Bool

func CFBundleIsExecutableLoadableForURL(CFURL!) -> Bool

func CFCopyHomeDirectoryURL() -> CFURL!

func CFDateFormatterCreateISO8601Formatter(CFAllocator!, CFISO8601DateFormatOptions) -> CFDateFormatter!

func CFFileSecurityClearProperties(CFFileSecurity!, CFFileSecurityClearOptions) -> Bool

Clears properties from a `CFFileSecurityRef` object.

func CFFileSecurityCopyAccessControlList(CFFileSecurity!, UnsafeMutablePointer&lt;acl_t?>!) -> Bool

Copies the access control list associated with a `CFFileSecurityRef` object.

func CFFileSecurityCopyGroupUUID(CFFileSecurity!, UnsafeMutablePointer&lt;Unmanaged&lt;CFUUID>?>!) -> Bool

Copies the group UUID associated with a `CFFileSecurityRef` object.

func CFFileSecurityCopyOwnerUUID(CFFileSecurity!, UnsafeMutablePointer&lt;Unmanaged&lt;CFUUID>?>!) -> Bool

Copies the owner UUID associated with a `CFFileSecurityRef` object.

