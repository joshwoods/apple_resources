

- Foundation
-  NSURL 

Class

# NSURL

An object that represents the location of a resource, such as an item on a remote server or the path to a local file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSURL
```

## Mentioned in 

Implementing Handoff in Your App

## Overview

In Swift, this object bridges to URL; use NSURL when you need reference semantics or other Foundation-specific behavior.

You can use URL objects to construct URLs and access their parts. For URLs that represent local files, you can also manipulate properties of those files directly, such as changing the file’s last modification date. Finally, you can pass URL objects to other APIs to retrieve the contents of those URLs. For example, you can use the URLSession, NSURLConnection, and NSURLDownload classes to access the contents of remote resources, as described in URL Loading System.

URL objects are the preferred way to refer to local files. Most objects that read data from or write data to a file have methods that accept an NSURL object instead of a pathname as the file reference. For example, you can get the contents of a local file URL as an `NSString` object using the init(contentsOfURL:encoding:) initializer, or as an `NSData` object using the init(contentsOfURL:options:) initializer.

You can also use URLs for interapplication communication. In macOS, the NSWorkspace class provides the open(_:) method to open a location specified by a URL. Similarly, in iOS, the UIApplication class provides the open(_:options:completionHandler:) method.

Additionally, you can use URLs when working with pasteboards, as described in NSURL Additions Reference (part of the AppKit framework).

The NSURL class is “toll-free bridged” with its Core Foundation counterpart, CFURL. See Toll-Free Bridging for more information on toll-free bridging.

Important

The Swift overlay to the Foundation framework provides the URL structure, which bridges to the NSURL class. For more information about value types, see Classes and Structures in The Swift Programming Language (Swift 4.1) and Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

### Structure of a URL

An NSURL object is composed of two parts—a potentially `nil` base URL and a string that is resolved relative to the base URL. An NSURL object is considered absolute if its string part is fully resolved without a base; all other URLs are considered relative.

For example, when constructing an `NSURL` object, you might specify `file:///path/to/user/` as the base URL and `folder/file.html` as the string part, as follows:

```
NSURL *baseURL = [NSURL fileURLWithPath:@"file:///path/to/user/"];
NSURL *URL = [NSURL URLWithString:@"folder/file.html" relativeToURL:baseURL];
NSLog(@"absoluteURL = %@", [URL absoluteURL]);
```

When fully resolved, the absolute URL is `file:///path/to/user/folder/file.html`.

A URL can be also be divided into pieces based on its structure. For example, the URL `https://johnny:p4ssw0rd@www.example.com:443/script.ext;param=value?query=value#ref` contains the following URL components:

| Component | Value |
|----|----|
| scheme | `https` |
| user | `johnny` |
| password | `p4ssw0rd` |
| host | `www.example.com` |
| port | `443` |
| path | `/script.ext` |
| pathExtension | `ext` |
| pathComponents | `["/", "script.ext"]` |
| parameterString | `param=value` |
| query | `query=value` |
| fragment | `ref` |

The NSURL class provides properties that let you examine each of these components.

Important

For apps linked on or after iOS 17 and aligned OS versions, NSURL parsing has updated from the obsolete RFC 1738/1808 parsing to the same RFC 3986 parsing as NSURLComponents. This unifies the parsing behaviors of the `NSURL` and `NSURLComponents` APIs. Now, `NSURL` automatically percent- and IDNA-encodes invalid characters to help create a valid URL.

To check if a `URLString` is strictly valid according to the RFC, use the new `[NSURL URLWithString:URLString encodingInvalidCharacters:NO]` method. This method leaves all characters as they are and returns `nil` if `URLString` is explicitly invalid.

For apps linked before iOS 17, the NSURL class parses URLs according to RFC 1808, RFC 1738, and RFC 2732.

### Bookmarks and Security Scope

Starting with OS X v10.6 and iOS 4.0, the NSURL class provides a facility for creating and using bookmark objects. A **bookmark** provides a persistent reference to a file-system resource. When you resolve a bookmark, you obtain a URL to the resource’s current location. A bookmark’s association with a file-system resource (typically a file or folder) usually continues to work if the user moves or renames the resource, or if the user relaunches your app or restarts the system.

For a general introduction to using bookmarks, read Locating Files Using Bookmarks in File System Programming Guide.

In a macOS app that adopts App Sandbox, you can use **security-scoped bookmarks** to gain access to file-system resources outside your app’s sandbox. These bookmarks preserve the user’s intent to give your app access to a resource across app launches. For details on how this works, including information on the entitlements you need in your Xcode project, read Security-Scoped Bookmarks and Persistent Resource Access in App Sandbox Design Guide. The methods for using security-scoped bookmarks are described in this document in Working with Bookmark Data.

When you resolve a security-scoped bookmark, you get a security-scoped URL.

### Security-Scoped URLs

Security-scoped URLs provide access to resources outside an app’s sandbox. In macOS, you get access to security-scoped URLs when you resolve a security-scoped bookmark. In iOS, apps that *open* or *move* documents using a UIDocumentPickerViewController also receive security-scoped URLs.

To gain access to a security-scoped URL, you must call the startAccessingSecurityScopedResource() method (or its Core Foundation equivalent, the CFURLStartAccessingSecurityScopedResource(_:) function). For iOS apps, if you use a UIDocument to access the URL, it automatically manages the security-scoped URL for you.

If `startAccessingSecurityScopedResource` (or `CFUrLStartAccessingSecurityScopedResource`) returns true, you must relinquish your access by calling the stopAccessingSecurityScopedResource() method (or its Core Foundation equivalent, the CFURLStopAccessingSecurityScopedResource(_:) function). You should relinquish your access as soon as you have finished using the file. After you call these methods, you immediately lose access to the resource in question.

Warning

If you fail to relinquish your access when you no longer need a file-system resource, your app leaks kernel resources. If sufficient kernel resources are leaked, your app loses its ability to add file-system locations to its sandbox, using Powerbox, security-scoped bookmarks, or similar APIs, until relaunched.

#### Security-Scoped URLs and String Paths

In a macOS app, when you copy a security-scoped URL, the copy has the security scope of the original. You gain access to the file-system resource (that the URL points to) just as you would with the original URL: by calling the startAccessingSecurityScopedResource() method (or its Core Foundation equivalent).

If you need a security-scoped URL’s path as a string value (as provided by the path method), such as to provide to an API that requires a string value, obtain the path from the URL as needed. Note, however, that a string-based path obtained from a security-scoped URL *does not* have security scope and you cannot use that string to obtain access to a security-scoped resource.

### iCloud Document Thumbnails

With OS X v10.10 and iOS 8.0, the NSURL class includes the ability to get and set document thumbnails as a resource property for iCloud documents. You can get a dictionary of NSImage objects in macOS or UIImage objects in iOS using the getResourceValue(_:forKey:) or getPromisedItemResourceValue(_:forKey:) methods.

- Swift
- Objective-C

```
let URL = self.URLForDocument()
var thumbnails: AnyObject?

do {
    try URL.getResourceValue(&thumbnails, forKey: NSURLThumbnailDictionaryKey)
    if let thumbnails = thumbnails as? [NSString: NSImage] {
        let image = thumbnails[NSThumbnail1024x1024SizeKey]
    }
} catch {
    // handle the error
}
```

```
NSURL *URL = [self URLForDocument];
NSDictionary *thumbnails = nil;
NSError *error = nil;

BOOL success = [URL getPromisedItemResourceValue:&thumbnails
                                          forKey:NSURLThumbnailDictionaryKey
                                           error:&error];
if (success) {
  NSImage *image = thumbnails[NSThumbnail1024x1024SizeKey];
} else {
  // handle the error
}
```

In macOS, you can set a dictionary of thumbnails using the setResourceValue(_:forKey:) method. You can also get or set all the thumbnails as an `NSImage` object with multiple representations by using the thumbnailKey.

- Swift
- Objective-C

```
let URL = self.URLForDocument()
let thumbnail = self.createDocumentThumbnail()

do {
    try URL.setResourceValue([NSThumbnail1024x1024SizeKey: thumbnail], forKey: NSURLThumbnailDictionaryKey)
} catch {
    // handle the error
}
```

```
NSURL *URL = [self URLForDocument];
NSImage *thumbnail = [self createDocumentThumbnail];
NSError *error = nil;

BOOL success = [URL setResourceValue:@{NSThumbnail1024x1024SizeKey : thumbnail}
                              forKey:NSURLThumbnailDictionaryKey
                               error:&error];

if (!success) {
  // handle the error
}
```

Note

Do not set the thumbnailDictionaryKey key directly. Modifying this key interferes with document tracking and can create duplicates of your document, as well as other possible problems.

In iOS, use a UIDocument subclass to manage your file. Set the thumbnail by overriding the document’s fileAttributesToWrite(to:for:) method and returning a dictionary that contains the proper thumbnail keys (along with any other file attributes).

In macOS, follow the instructions for creating thumbnails given in Quick Look Programming Guide.

Note

Although the thumbnail API is designed to support multiple image resolutions, currently it only supports 1024 x 1024 pixel thumbnails.

## Topics

### Creating a URL object

convenience init?(string: String)

Initializes an NSURL object with a provided URL string.

convenience init?(string: String, encodingInvalidCharacters: Bool)

Creates an instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

init?(string: String, relativeTo: URL?)

Initializes an NSURL object with a base URL and a relative string.

class func fileURL(withPath: String, isDirectory: Bool) -> URL

Initializes and returns a newly created NSURL object as a file URL with a specified path.

init(fileURLWithPath: String, isDirectory: Bool)

Initializes a newly created NSURL referencing the local file or directory at `path`.

class func fileURL(withPath: String, relativeTo: URL?) -> URL

init(fileURLWithPath: String, relativeTo: URL?)

class func fileURL(withPath: String, isDirectory: Bool, relativeTo: URL?) -> URL

init(fileURLWithPath: String, isDirectory: Bool, relativeTo: URL?)

class func fileURL(withPath: String) -> URL

Initializes and returns a newly created NSURL object as a file URL with a specified path.

init(fileURLWithPath: String)

Initializes a newly created NSURL referencing the local file or directory at `path`.

class func fileURL(withPathComponents: [String]) -> URL?

Initializes and returns a newly created NSURL object as a file URL with specified path components.

convenience init(resolvingAliasFileAt: URL, options: NSURL.BookmarkResolutionOptions) throws

Returns a new URL made by resolving the alias file at `url`.

convenience init(resolvingBookmarkData: Data, options: NSURL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: UnsafeMutablePointer&lt;ObjCBool>?) throws

Initializes a newly created NSURL that points to a location specified by resolving bookmark data.

class func fileURL(withFileSystemRepresentation: UnsafePointer&lt;CChar>, isDirectory: Bool, relativeTo: URL?) -> URL

Returns a new URL object initialized with a C string representing a local file system path.

func getFileSystemRepresentation(UnsafeMutablePointer&lt;CChar>, maxLength: Int) -> Bool

Fills the provided buffer with a C string representing a local file system path.

init(fileURLWithFileSystemRepresentation: UnsafePointer&lt;CChar>, isDirectory: Bool, relativeTo: URL?)

Initializes a URL object with a C string representing a local file system path.

class func absoluteURL(withDataRepresentation: Data, relativeTo: URL?) -> URL

init(absoluteURLWithDataRepresentation: Data, relativeTo: URL?)

init(dataRepresentation: Data, relativeTo: URL?)

var dataRepresentation: Data

### Querying an NSURL

func checkResourceIsReachableAndReturnError(NSErrorPointer) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

func isFileReferenceURL() -> Bool

Returns whether the URL is a file reference URL.

var isFileURL: Bool

A boolean value that determines whether the receiver is a file URL.

### Accessing the Parts of the URL

var absoluteString: String?

The URL string for the receiver as an absolute URL. (read-only)

var absoluteURL: URL?

An absolute URL that refers to the same resource as the receiver. (read-only)

var baseURL: URL?

The base URL. (read-only)

var fileSystemRepresentation: UnsafePointer&lt;CChar>

A C string containing the URL’s file system path. (read-only)

var fragment: String?

The fragment identifier, conforming to RFC 1808. (read-only)

var host: String?

The host, conforming to RFC 1808. (read-only)

var lastPathComponent: String?

The last path component. (read-only)

var parameterString: String?

The parameter string conforming to RFC 1808. (read-only)

Deprecated

var password: String?

The password conforming to RFC 1808. (read-only)

var path: String?

The path, conforming to RFC 1808. (read-only)

var pathComponents: [String]?

An array containing the path components. (read-only)

var pathExtension: String?

The path extension. (read-only)

var port: NSNumber?

The port, conforming to RFC 1808.

var query: String?

The query string, conforming to RFC 1808.

var relativePath: String?

The relative path, conforming to RFC 1808. (read-only)

var relativeString: String

A string representation of the relative portion of the URL. (read-only)

var resourceSpecifier: String?

The resource specifier. (read-only)

var scheme: String?

The scheme. (read-only)

var standardized: URL?

A copy of the URL with any instances of `".."` or `"."` removed from its path. (read-only)

var user: String?

The user name, conforming to RFC 1808.

### Accessing Resource Values

func resourceValues(forKeys: [URLResourceKey]) throws -> [URLResourceKey : Any]

Returns the resource values for the properties identified by specified array of keys.

func getResourceValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: URLResourceKey) throws

Returns the value of the resource property for the specified key.

func setResourceValue(Any?, forKey: URLResourceKey) throws

Sets the URL’s resource property for a given key to a given value.

func setResourceValues([URLResourceKey : Any]) throws

Sets the URL’s resource properties for a given set of keys to a given set of values.

func removeAllCachedResourceValues()

Removes all cached resource values and temporary resource values from the URL object.

func removeCachedResourceValue(forKey: URLResourceKey)

Removes the cached resource value identified by a given key from the URL object.

func setTemporaryResourceValue((any Sendable)?, forKey: URLResourceKey)

Sets a temporary resource value on the URL object.

struct URLResourceKey

Keys that apply to file system URLs.

### Modifying and Converting a File URL

var filePathURL: URL?

A file path URL that points to the same resource as the URL object. (read-only)

func fileReferenceURL() -> URL?

Returns a new file reference URL that points to the same resource as the receiver.

func appendingPathComponent(String) -> URL?

Returns a new URL by appending a path component to the original URL.

func appendingPathComponent(String, isDirectory: Bool) -> URL?

Returns a new URL by appending a path component to the original URL, along with a trailing slash if the component is a directory.

func appendingPathComponent(String, conformingTo: UTType) -> URL

Returns a URL by appending the specified path component with the file extension for a uniform type identifier.

func appendingPathExtension(String) -> URL?

Returns a new URL by appending a path extension to the original URL.

func appendingPathExtension(for: UTType) -> URL

Returns a URL by appending the path extension for a uniform type identifier.

var deletingLastPathComponent: URL?

A URL you create by removing the last path component from the receiver. (read-only)

var deletingPathExtension: URL?

A URL you create by removing the path extension from the receiver, if any. (read-only)

var resolvingSymlinksInPath: URL?

A URL that points to the same resource as the receiver and includes no symbolic links. (read-only)

var standardizingPath: URL?

A URL that points to the same resource as the original URL using an absolute path. (read-only)

var hasDirectoryPath: Bool

A Boolean value that indicates whether the URL string’s path represents a directory.

### Working with Bookmark Data

class func bookmarkData(withContentsOf: URL) throws -> Data

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

func bookmarkData(options: NSURL.BookmarkCreationOptions, includingResourceValuesForKeys: [URLResourceKey]?, relativeTo: URL?) throws -> Data

Returns a bookmark for the URL, created with specified options and resource values.

class func resourceValues(forKeys: [URLResourceKey], fromBookmarkData: Data) -> [URLResourceKey : Any]?

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

class func writeBookmarkData(Data, to: URL, options: NSURL.BookmarkFileCreationOptions) throws

Creates an alias file on disk at a specified location with specified bookmark data.

func startAccessingSecurityScopedResource() -> Bool

In an app that has adopted App Sandbox, makes the resource pointed to by a security-scoped URL available to the app.

func stopAccessingSecurityScopedResource()

In an app that adopts App Sandbox, revokes access to the resource pointed to by a security-scoped URL.

typealias BookmarkFileCreationOptions

Options used when creating file bookmark data

struct BookmarkCreationOptions

Options used when creating bookmark data.

struct BookmarkResolutionOptions

Options used when resolving bookmark data.

### Working with Promised Items

func checkPromisedItemIsReachableAndReturnError(NSErrorPointer) -> Bool

Returns whether the promised item can be reached.

func getPromisedItemResourceValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: URLResourceKey) throws

Returns the value of the resource property for the specified key.

func promisedItemResourceValues(forKeys: [URLResourceKey]) throws -> [URLResourceKey : Any]

Returns the resource values for the properties identified by specified array of keys.

### Working with Pasteboards

init?(fromPasteboard: NSPasteboard)

Reads an NSURL object off of the specified pasteboard.

func write(to: NSPasteboard)

Writes the URL to the specified pasteboard.

### Using Quick Looks

var customPlaygroundQuickLook: PlaygroundQuickLookDeprecated

### Constants

NSURL Schemes

The schemes that the `NSURL` class is able to parse.

NSError userInfo Dictionary Keys

Keys in the userInfo dictionary of an `NSError` object when certain NSURL methods return an error.

### Deprecated

convenience init?(scheme: String, host: String?, path: String)

Initializes a newly created NSURL with a specified scheme, host, and path.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSObjectProtocol
- NSPasteboardReading
- NSPasteboardWriting
- NSSecureCoding
- QLPreviewItem
- Sendable

