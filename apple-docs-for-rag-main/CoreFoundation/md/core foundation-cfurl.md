

- Core Foundation
-  CFURL 

Class

# CFURL

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFURL
```

## Overview

The `CFURL` opaque type provides facilities for creating, parsing, and dereferencing URL strings. `CFURL` is useful to applications that need to use URLs to access resources, including local files.

A `CFURL` object is composed of two parts—a base URL, which can be `NULL`, and a string that is resolved relative to the base URL. A `CFURL` object whose string is fully resolved without a base URL is considered absolute; all others are considered relative.

`CFURL` is “toll-free bridged” with its Cocoa Foundation counterpart, NSURL. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. In other words, in a method where you see an `NSURL *` parameter, you can pass in a `CFURLRef`, and in a function where you see a `CFURLRef` parameter, you can pass in an `NSURL` instance. This also applies to concrete subclasses of `NSURL`. See Toll-Free Bridged Types for more information on toll-free bridging.

Starting in OS X v10.6, the `CFURL` opaque type provides a facility for creating and using bookmarks. A *bookmark* provides a persistent reference to a file-system resource. When you resolve a bookmark, you obtain a URL to the resource’s current location. A bookmark’s association with a file-system resource (typically a file or folder) usually continues to work if the user moves or renames the resource, or if the user relaunches your app or restarts the system.

In a macOS app that adopts App Sandbox, to gain persistent access to a file-system resource you must use a *security-scoped bookmark*. Such a bookmark preserves, across app launches, a user’s intent to give your app access to a resource. For details on how this works, including information on the entitlements you need in your Xcode project, read Security-Scoped Bookmarks and Persistent Resource Access in App Sandbox Design Guide.

When you resolve a security-scoped bookmark, you get a security-scoped URL. The file system resource that the URL points to is not available for use inside your app’s sandbox until you call the CFURLStartAccessingSecurityScopedResource(_:) function (or its Cocoa equivalent, the startAccessingSecurityScopedResource() method) on the URL.

When you no longer need access to a resource that you obtained using security scope (typically, after you close the resource) you must call the CFURLStopAccessingSecurityScopedResource(_:) method (or its Cocoa equivalent, the stopAccessingSecurityScopedResource() method) on the resource’s URL.

Warning

You must balance every call to the CFURLStartAccessingSecurityScopedResource(_:) method with a corresponding call to the CFURLStopAccessingSecurityScopedResource(_:) method. If you fail to relinquish your access when you no longer need a file-system resource, your app leaks kernel resources. If sufficient kernel resources are leaked, your app loses its ability to add file-system locations to its sandbox, such as via Powerbox or security-scoped bookmarks, until relaunched.

The functions for using security-scoped bookmarks are described in this document in Working with Bookmark Data. For a general introduction to using bookmarks in macOS, read Locating Files Using Bookmarks in File System Programming Guide.

When you copy a security-scoped URL (as obtained from a security-scoped bookmark), the copy has the security scope of the original. You gain access to the file-system resource (that the URL points to) just as you would with the original URL: by calling the CFURLStartAccessingSecurityScopedResource(_:) function (or its Cocoa equivalent).

If you need a security-scoped URL’s path as a string value (as provided by the CFURLGetString(_:) function), such as to provide to an API that requires a string value, obtain the path from the URL as needed. Note, however, that a string-based path obtained from a security-scoped URL *does not* have security scope and you cannot use that string to obtain access a security-scoped resource.

`CFURL` fails to create an object if the string passed is not well-formed (that is, if it does not comply with RFC 2396). Examples of cases that will not succeed are strings containing space characters and high-bit characters. If a function fails to create a `CFURL` object, it returns `NULL`, which you must be prepared to handle. If you create `CFURL` objects using file system paths, you should use the CFURLCreateFromFileSystemRepresentation(_:_:_:_:) and CFURLCreateFromFileSystemRepresentationRelativeToBase(_:_:_:_:_:) functions, which handle the subtle differences between URL paths and file system paths.

For functions that read and write data from a URL, see Core Foundation URL Access Utilities

## Topics

### Creating a CFURL

func CFURLCopyAbsoluteURL(CFURL!) -> CFURL!

Creates a new `CFURL` object by resolving the relative portion of a URL against its base.

func CFURLCreateAbsoluteURLWithBytes(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, CFURL!, Bool) -> CFURL!

Creates a new `CFURL` object by resolving the relative portion of a URL, specified as bytes, against its given base URL.

func CFURLCreateByResolvingBookmarkData(CFAllocator!, CFData!, CFURLBookmarkResolutionOptions, CFURL!, CFArray!, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFURL>!

Returns a new URL made by resolving bookmark data.

func CFURLCreateCopyAppendingPathComponent(CFAllocator!, CFURL!, CFString!, Bool) -> CFURL!

Creates a copy of a given URL and appends a path component.

func CFURLCreateCopyAppendingPathExtension(CFAllocator!, CFURL!, CFString!) -> CFURL!

Creates a copy of a given URL and appends a path extension.

func CFURLCreateCopyDeletingLastPathComponent(CFAllocator!, CFURL!) -> CFURL!

Creates a copy of a given URL with the last path component deleted.

func CFURLCreateCopyDeletingPathExtension(CFAllocator!, CFURL!) -> CFURL!

Creates a copy of a given URL with its last path extension removed.

func CFURLCreateFilePathURL(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFURL>!

Returns a new file path URL that refers to the same resource as a specified URL.

func CFURLCreateFileReferenceURL(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFURL>!

Returns a new file reference URL that points to the same resource as a specified URL.

func CFURLCreateFromFileSystemRepresentation(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, Bool) -> CFURL!

Creates a new `CFURL` object for a file system entity using the native representation.

func CFURLCreateFromFileSystemRepresentationRelativeToBase(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, Bool, CFURL!) -> CFURL!

Creates a `CFURL` object from a native character string path relative to a base URL.

func CFURLCreateFromFSRef(CFAllocator!, OpaquePointer!) -> CFURL!

Creates a URL from a given directory or file.

Deprecated

func CFURLCreateWithBytes(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, CFURL!) -> CFURL!

Creates a `CFURL` object using a given character bytes.

func CFURLCreateWithFileSystemPath(CFAllocator!, CFString!, CFURLPathStyle, Bool) -> CFURL!

Creates a `CFURL` object using a local file system path string.

func CFURLCreateWithFileSystemPathRelativeToBase(CFAllocator!, CFString!, CFURLPathStyle, Bool, CFURL!) -> CFURL!

Creates a `CFURL` object using a local file system path string relative to a base URL.

func CFURLCreateWithString(CFAllocator!, CFString!, CFURL!) -> CFURL!

Creates a `CFURL` object using a given `CFString` object.

### Accessing the Parts of a URL

func CFURLCanBeDecomposed(CFURL!) -> Bool

Determines if the given URL conforms to RFC 1808 and therefore can be decomposed.

func CFURLCopyFileSystemPath(CFURL!, CFURLPathStyle) -> CFString!

Returns the path portion of a given URL.

func CFURLCopyFragment(CFURL!, CFString!) -> CFString!

Returns the fragment from a given URL.

func CFURLCopyHostName(CFURL!) -> CFString!

Returns the host name of a given URL.

func CFURLCopyLastPathComponent(CFURL!) -> CFString!

Returns the last path component of a given URL.

func CFURLCopyNetLocation(CFURL!) -> CFString!

Returns the net location portion of a given URL.

func CFURLCopyParameterString(CFURL!, CFString!) -> CFString!

Returns the parameter string from a given URL.

Deprecated

func CFURLCopyPassword(CFURL!) -> CFString!

Returns the password of a given URL.

func CFURLCopyPath(CFURL!) -> CFString!

Returns the path portion of a given URL.

func CFURLCopyPathExtension(CFURL!) -> CFString!

Returns the path extension of a given URL.

func CFURLCopyQueryString(CFURL!, CFString!) -> CFString!

Returns the query string of a given URL.

func CFURLCopyResourceSpecifier(CFURL!) -> CFString!

Returns any additional resource specifiers after the path.

func CFURLCopyScheme(CFURL!) -> CFString!

Returns the scheme portion of a given URL.

func CFURLCopyStrictPath(CFURL!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> CFString!

Returns the path portion of a given URL.

func CFURLCopyUserName(CFURL!) -> CFString!

Returns the user name from a given URL.

func CFURLGetPortNumber(CFURL!) -> Int32

Returns the port number from a given URL.

func CFURLHasDirectoryPath(CFURL!) -> Bool

Determines if a given URL’s path represents a directory.

### Converting URLs to Other Representations

func CFURLCreateData(CFAllocator!, CFURL!, CFStringEncoding, Bool) -> CFData!

Creates a `CFData` object containing the content of a given URL.

func CFURLCreateStringByAddingPercentEscapes(CFAllocator!, CFString!, CFString!, CFString!, CFStringEncoding) -> CFString!

Creates a copy of a string, replacing certain characters with the equivalent percent escape sequence based on the specified encoding.

Deprecated

func CFURLCreateStringByReplacingPercentEscapes(CFAllocator!, CFString!, CFString!) -> CFString!

Creates a new string by replacing any percent escape sequences with their character equivalent.

func CFURLCreateStringByReplacingPercentEscapesUsingEncoding(CFAllocator!, CFString!, CFString!, CFStringEncoding) -> CFString!

Creates a new string by replacing any percent escape sequences with their character equivalent.

Deprecated

func CFURLGetFileSystemRepresentation(CFURL!, Bool, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> Bool

Fills a buffer with the file system’s native string representation of a given URL’s path.

func CFURLGetFSRef(CFURL!, OpaquePointer!) -> Bool

Converts a given URL to a file or directory object.

Deprecated

func CFURLGetString(CFURL!) -> CFString!

Returns the URL as a `CFString` object.

### Getting URL Properties

func CFURLGetBaseURL(CFURL!) -> CFURL!

Returns the base URL of a given URL if it exists.

func CFURLGetBytes(CFURL!, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> CFIndex

Returns by reference the byte representation of a URL object.

func CFURLGetByteRangeForComponent(CFURL!, CFURLComponentType, UnsafeMutablePointer&lt;CFRange>!) -> CFRange

Returns the range of the specified component in the bytes of a URL.

func CFURLGetTypeID() -> CFTypeID

Returns the type identifier for the `CFURL` opaque type.

func CFURLResourceIsReachable(CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

### Getting and Setting File System Resource Properties

func CFURLClearResourcePropertyCache(CFURL!)

Removes all cached resource values and temporary resource values from the URL object.

func CFURLClearResourcePropertyCacheForKey(CFURL!, CFString!)

Removes the cached resource value identified by a given key from the URL object.

func CFURLCopyResourcePropertiesForKeys(CFURL!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

Returns the resource values for the properties identified by specified array of keys.

func CFURLCopyResourcePropertyForKey(CFURL!, CFString!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns the value of a given resource property of a given URL.

func CFURLCreateResourcePropertiesForKeysFromBookmarkData(CFAllocator!, CFArray!, CFData!) -> Unmanaged&lt;CFDictionary>!

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

func CFURLCreateResourcePropertyForKeyFromBookmarkData(CFAllocator!, CFString!, CFData!) -> Unmanaged&lt;CFTypeRef>!

Returns the value of a resource property from specified bookmark data.

func CFURLSetResourcePropertiesForKeys(CFURL!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the URL’s resource properties for a given set of keys to a given set of values.

func CFURLSetResourcePropertyForKey(CFURL!, CFString!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the URL’s resource property for a given key to a given value.

func CFURLSetTemporaryResourcePropertyForKey(CFURL!, CFString!, CFTypeRef!)

Sets a temporary resource value on the URL.

### Working with Bookmark Data

func CFURLCreateBookmarkData(CFAllocator!, CFURL!, CFURLBookmarkCreationOptions, CFArray!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns bookmark data for a URL, created with specified options and resource values.

func CFURLCreateBookmarkDataFromAliasRecord(CFAllocator!, CFData!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from an alias record.

Deprecated

func CFURLCreateBookmarkDataFromFile(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from a file pointed to by a specified URL.

func CFURLWriteBookmarkDataToFile(CFData!, CFURL!, CFURLBookmarkFileCreationOptions, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Creates an alias file on disk at a specified location with specified bookmark data.

func CFURLStartAccessingSecurityScopedResource(CFURL!) -> Bool

In an app that has adopted App Sandbox, makes the resource pointed to by a security-scoped URL available to the app.

func CFURLStopAccessingSecurityScopedResource(CFURL!)

In an app that adopts App Sandbox, revokes access to the resource pointed to by a security-scoped URL.

### Bookmark Data Types

struct CFURLBookmarkCreationOptions

Type for bookmark data creation options.

typealias CFURLBookmarkFileCreationOptions

Type for bookmark file creation options.

struct CFURLBookmarkResolutionOptions

Type for bookmark data resolution options.

### Bookmark Data Constants

Bookmark Data Creation Options

Options used when creating bookmark data.

Bookmark Data Resolution Options

Options used when resolving bookmark data.

### File System Constants

Common File System Resource Keys

Keys that are applicable to file system URLs.

File Resource Types

Possible values for the kCFURLFileResourceTypeKey key.

File Property Keys

Keys that apply to properties of files.

iCloud Constants

These constants can be used to determining whether a file is stored in the cloud and to obtain information about its status.

Volume Property Keys

Keys that apply to volumes.

CFError userInfo Dictionary Keys

Keys in the userInfo dictionary of a `CFError` object when certain CFURL functions return an error.

### Miscellaneous

enum CFURLComponentType

The types of components in a URL.

enum CFURLPathStyle

Options you can use to determine how CFURL functions parse a file system path name.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

