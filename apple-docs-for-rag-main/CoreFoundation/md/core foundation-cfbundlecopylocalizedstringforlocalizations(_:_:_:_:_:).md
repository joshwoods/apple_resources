

- Core Foundation
-  CFBundleCopyLocalizedStringForLocalizations(\_:\_:\_:\_:\_:) 

Function

# CFBundleCopyLocalizedStringForLocalizations(\_:\_:\_:\_:\_:)

Returns a localized string from a bundle’s strings file.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func CFBundleCopyLocalizedStringForLocalizations(
    _ bundle: CFBundle!,
    _ key: CFString!,
    _ value: CFString!,
    _ tableName: CFString!,
    _ localizations: CFArray!
) -> CFString!
```

## Parameters 

`bundle`  

The bundle to examine.

`key`  

The key for the localized string to retrieve. This key will be used to look up the localized string in the strings file. Typically the key is identical to the value of the localized string in the development language.

`value`  

A default value to return if no value exists for `key`.

`tableName`  

The name of the strings file to search. The name should not include the `strings` filename extension. The case of the string must match that of the file name, even on file systems (such as HFS+) that are not case sensitive with regards to file names

`localizations`  

An array of BCP 47 language codes corresponding to available localizations. Bundle compares the array against its available localizations, and uses the best result to retrieve the localized string. If empty, we treat it as no localization is available, and may return a fallback.

## Return Value

A CFString object that contains the localized string. If no value exists for `key`, returns `value` unless `value` is `NULL` or an empty string, in which case `key` is returned instead. Ownership follows the The Create Rule.

## Discussion

Returns a localized string given a list of possible localizations. The one most suitable to use with the given `bundle` is returned.

## See Also

### Functions

func CFAllocatorAllocateBytes(CFAllocator!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

func CFAllocatorAllocateTyped(CFAllocator!, CFIndex, CFAllocatorTypeID, CFOptionFlags) -> UnsafeMutableRawPointer!

func CFAllocatorReallocateBytes(CFAllocator!, UnsafeMutableRawPointer!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

func CFAllocatorReallocateTyped(CFAllocator!, UnsafeMutableRawPointer!, CFIndex, CFAllocatorTypeID, CFOptionFlags) -> UnsafeMutableRawPointer!

func CFAttributedStringGetBidiLevelsAndResolvedDirections(CFAttributedString!, CFRange, Int8, UnsafeMutablePointer&lt;UInt8>!, UnsafeMutablePointer&lt;UInt8>!) -> Bool

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

func CFFileSecurityCreate(CFAllocator!) -> CFFileSecurity!

Creates a `CFFileSecurityRef` object.

