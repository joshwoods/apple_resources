

- Core Foundation
-  CFURLEnumeratorCreateForMountedVolumes(\_:\_:\_:) 

Function

# CFURLEnumeratorCreateForMountedVolumes(\_:\_:\_:)

Creates and returns a volume enumerator with provided enumerator behavior options and properties to be prefetched.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLEnumeratorCreateForMountedVolumes(
    _ alloc: CFAllocator!,
    _ option: CFURLEnumeratorOptions,
    _ propertyKeys: CFArray!
) -> CFURLEnumerator!
```

## Parameters 

`alloc`  

The memory allocator to use. If `NULL`, the default allocator is used.

`option`  

A bit array of enumerator behavior options.

`propertyKeys`  

An array of file property keys to prefetch for each enumerated URL. Can be `NULL`.

## Return Value

The created volume enumerator.

## Discussion

Volume enumerators generate file path URLs by default. To generate file reference URLs instead, include the generateFileReferenceURLs option in `options`.

Specifying prefetch properties allows the enumerator to optimize device access by using bulk operations. However, you should not prefetch properties that are not needed, because doing so may degrade performance.

This function ignores the descendRecursively and skipPackageContents options.

## See Also

### Related Documentation

struct CFURLEnumeratorOptions

Options for controlling enumerator behavior.

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

