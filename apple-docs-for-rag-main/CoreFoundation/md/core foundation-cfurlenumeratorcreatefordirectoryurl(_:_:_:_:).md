

- Core Foundation
-  CFURLEnumeratorCreateForDirectoryURL(\_:\_:\_:\_:) 

Function

# CFURLEnumeratorCreateForDirectoryURL(\_:\_:\_:\_:)

Creates and returns a directory enumerator with provided enumerator behavior options and properties to be prefetched.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLEnumeratorCreateForDirectoryURL(
    _ alloc: CFAllocator!,
    _ directoryURL: CFURL!,
    _ option: CFURLEnumeratorOptions,
    _ propertyKeys: CFArray!
) -> CFURLEnumerator!
```

## Parameters 

`alloc`  

The memory allocator to use. If `NULL`, the default allocator is used.

`directoryURL`  

The URL of the directory to enumerate.

`option`  

A bit array of enumerator behavior options.

`propertyKeys`  

An array of file property keys to prefetch for each enumerated URL. Can be `NULL`.

## Return Value

The created directory enumerator.

## Discussion

Directory enumerators do not descend into subdirectories of `directoryURL` by default. To create a recursive enumerator, include the descendRecursively option in `options`.

Specifying prefetch properties allows the enumerator to optimize device access by using bulk operations. However, you should not prefetch properties that are not needed, because doing so may degrade performance.

The created directory enumerator generates URLs with the same type as `directoryURL`. If `directoryURL` is a file reference URL, then enumerated URLs are file reference URLs. If `directoryURL` is a file path URL, then enumerated URLs are file path URLs.

In some areas of the file system hierarchy, file reference URLs cannot be generated. The enumerator always generates file path URLs for these areas.

This function ignores the generateFileReferenceURLs option.

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

