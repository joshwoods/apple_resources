

- Core Foundation
-  CFFileSecurityCreateCopy(\_:\_:) 

Function

# CFFileSecurityCreateCopy(\_:\_:)

Creates a copy of a `CFFileSecurityRef` object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileSecurityCreateCopy(
    _ allocator: CFAllocator!,
    _ fileSec: CFFileSecurity!
) -> CFFileSecurity!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`fileSec`  

The `CFFileSecurityRef` object to copy.

## Return Value

Returns a new `CFFileSecurityRef` object, or `NULL` if an error occurred. Ownership follows the Create Rule.

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

