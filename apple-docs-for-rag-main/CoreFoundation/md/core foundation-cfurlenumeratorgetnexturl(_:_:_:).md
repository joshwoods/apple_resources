

- Core Foundation
-  CFURLEnumeratorGetNextURL(\_:\_:\_:) 

Function

# CFURLEnumeratorGetNextURL(\_:\_:\_:)

Advances an enumerator to the next URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLEnumeratorGetNextURL(
    _ enumerator: CFURLEnumerator!,
    _ url: UnsafeMutablePointer?>!,
    _ error: UnsafeMutablePointer?>!
) -> CFURLEnumeratorResult
```

## Parameters 

`enumerator`  

The enumerator.

`url`  

Contains the next URL if this function returns CFURLEnumeratorResult.success.

`error`  

Contains error information if this function returns CFURLEnumeratorResult.error. Error information is retained and must be released. Can be `NULL`.

## Return Value

The result of advancing the enumerator.

## Discussion

If this function returns CFURLEnumeratorResult.end, the enumeration has finished.

A return value of CFURLEnumeratorResult.error does not imply that the enumeration has finished.

If this function returns CFURLEnumeratorResult.error, the user info dictionary of `error` is populated with the following entries (when possible):

- The kCFErrorUnderlyingErrorKey entry is populated with the underlying error if the underlying error is not in the kCFErrorDomainCocoa domain.

- The NSURLErrorKey entry is populated with the URL that caused the error, as a CFURL object.

- The NSFilePathErrorKey entry is populated with the file path that caused the error, as a CFString object.

## See Also

### Related Documentation

enum CFURLEnumeratorResult

Result codes from the CFURLEnumeratorGetNextURL(_:_:_:) function.

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

