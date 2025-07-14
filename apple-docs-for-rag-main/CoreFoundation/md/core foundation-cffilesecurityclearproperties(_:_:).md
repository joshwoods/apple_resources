

- Core Foundation
-  CFFileSecurityClearProperties(\_:\_:) 

Function

# CFFileSecurityClearProperties(\_:\_:)

Clears properties from a `CFFileSecurityRef` object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileSecurityClearProperties(
    _ fileSec: CFFileSecurity!,
    _ clearPropertyMask: CFFileSecurityClearOptions
) -> Bool
```

## Parameters 

`fileSec`  

The file security properties to clear.

`clearPropertyMask`  

The file security properties to clear.

## Return Value

Returns `true` if the file security properties were successfully cleared, or `false` otherwise.

## Discussion

One common use for `CFFileSecurityRef` objects is to clone the permissions from one file to another. In this use, you may want to copy only a subset of the permissions. This function lets you delete the specific permissions that you do not want to change prior to applying the set of permissions to a different file.

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

func CFFileSecurityCopyAccessControlList(CFFileSecurity!, UnsafeMutablePointer&lt;acl_t?>!) -> Bool

Copies the access control list associated with a `CFFileSecurityRef` object.

func CFFileSecurityCopyGroupUUID(CFFileSecurity!, UnsafeMutablePointer&lt;Unmanaged&lt;CFUUID>?>!) -> Bool

Copies the group UUID associated with a `CFFileSecurityRef` object.

func CFFileSecurityCopyOwnerUUID(CFFileSecurity!, UnsafeMutablePointer&lt;Unmanaged&lt;CFUUID>?>!) -> Bool

Copies the owner UUID associated with a `CFFileSecurityRef` object.

func CFFileSecurityCreate(CFAllocator!) -> CFFileSecurity!

Creates a `CFFileSecurityRef` object.

