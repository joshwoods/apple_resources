

- Foundation
-  URL 

Structure

# URL

A value that identifies the location of a resource, such as an item on a remote server or the path to a local file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct URL
```

## Mentioned in 

Downloading files from websites

Checking Volume Storage Capacity

Processing URL session data task results with Combine

Encoding and Decoding Custom Types

## Overview

You can construct URLs and access their parts. For URLs that represent local files, you can also manipulate properties of those files directly, such as changing the file’s last modification date. Finally, you can pass URLs to other APIs to retrieve the contents of those URLs. For example, you can use URLSession and its related classes to access the contents of remote resources.

URLs are the preferred way to refer to local files. Most objects that read data from or write data to a file have methods that accept a URL instead of a pathname as the file reference. For example, you can get the contents of a local file URL as String by calling init(contentsOf:encoding:), or as a Data by calling init(contentsOf:options:).

As a convenience, you can use Swift’s `async`-`await` syntax to asynchronously access the contents of a URL through the resourceBytes and lines properties. These properties use the shared URLSession instance to load the resource.

## Topics

### Creating a URL from a string

init?(string: String)

Creates a URL instance from the provided string.

init?(string: String, encodingInvalidCharacters: Bool)

Creates a URL instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

init?(string: String, relativeTo: URL?)

Creates a URL instance from the provided string, relative to another URL.

init(resolvingBookmarkData: Data, options: URL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: inout Bool) throws

Creates a URL that refers to a location specified by resolving bookmark data.

init?(resolvingBookmarkData: Data, options: URL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: inout Bool) throws

Initializes a URL that refers to a location specified by resolving bookmark data.

### Creating a file URL from a string path

init(filePath: String, directoryHint: URL.DirectoryHint, relativeTo: URL?)

Creates a file URL that references a path you specify as a string.

enum DirectoryHint

A hint to URL file APIs for handling paths that may reference directories.

init(fileURLWithPath: String)

Creates a file URL that references the local file or directory at the given path.

Deprecated

init(fileURLWithPath: String, isDirectory: Bool)

Creates a file URL that references the local file or directory at the given path.

Deprecated

init(fileURLWithPath: String, relativeTo: URL?)

Creates a file URL that references the local file or directory at the given path, relative to a base URL.

Deprecated

init(fileURLWithPath: String, isDirectory: Bool, relativeTo: URL?)

Creates a file URL that references the local file or directory at the given path, relative to a base URL.

Deprecated

init(fileURLWithFileSystemRepresentation: UnsafePointer&lt;Int8>, isDirectory: Bool, relativeTo: URL?)

Creates a file URL that references the local file or directory for the file system representation of the path.

init(fileReferenceLiteralResourceName: String)

Creates a URL from a playground file literal.

init?(filePath: FilePath, directoryHint: URL.DirectoryHint)

Creates a file URL that references a file path.

### Creating a file URL from a file path

init?(FilePath)

Creates a file URL that references the local file or directory at the file path you specify.

Deprecated

init?(FilePath, isDirectory: Bool)

Creates a file URL that references the local file or directory at the file path you specify.

Deprecated

struct FilePath

Represents a location in the file system.

### Creating a file URL for a common directory

init(for: FileManager.SearchPathDirectory, in: FileManager.SearchPathDomainMask, appropriateFor: URL?, create: Bool) throws

Creates a file URL for a common directory in a domain.

enum SearchPathDirectory

The location of significant directories.

struct SearchPathDomainMask

Domain constants specifying base locations to use when you search for significant directories.

### Creating a URL by resolving a bookmark

init(resolvingBookmarkData: Data, options: URL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: inout Bool) throws

Creates a URL that refers to a location specified by resolving bookmark data.

init(resolvingAliasFileAt: URL, options: URL.BookmarkResolutionOptions) throws

Creates a URL that refers to the location specified by resolving an alias file.

typealias BookmarkResolutionOptions

An alias for the bookmark resolution options type.

struct BookmarkResolutionOptions

Options used when resolving bookmark data.

### Creating a URL from a resource

init?(resource: URLResource)

Creates a URL from a resource.

### Creating a URL by parsing

init&lt;T>(T.ParseInput, strategy: T) throws

Creates a URL instance by parsing the provided input in accordance with a parse strategy.

struct ParseStrategy

A parse strategy for creating URLs from formatted strings.

### Accessing the parts of a URL

func fragment(percentEncoded: Bool) -> String?

Returns the fragment component of the URL, optionally removing any percent-encoding.

var fragment: String?

The fragment component of the URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

func host(percentEncoded: Bool) -> String?

Returns the host component of the URL, optionally removing any percent-encoding.

var host: String?

The host component of a URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

var lastPathComponent: String

The last path component of the URL, or an empty string if the path is an empty string.

func path(percentEncoded: Bool) -> String

Returns the path component of the URL, optionally removing any percent-encoding.

var path: String

The path component of the URL if the URL conforms to RFC 3986; otherwise, an empty string.

Deprecated

func password(percentEncoded: Bool) -> String?

Returns the password component of the URL, optionally removing any percent-encoding.

var password: String?

The password component of the URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

var pathComponents: [String]

The path components of the URL, or an empty array if the path is an empty string.

var pathExtension: String

The path extension of the URL, or an empty string if the path is an empty string.

var port: Int?

The port component of the URL if the URL conforms to RFC 3986; otherwise, nil.

func query(percentEncoded: Bool) -> String?

Returns the query component of the URL, optionally removing any percent-encoding.

var query: String?

The query of the URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

var scheme: String?

The scheme of the URL.

func user(percentEncoded: Bool) -> String?

Returns the user component of the URL, optionally removing any percent-encoding.

var user: String?

The user component of the URL if the URL conforms to RFC 3986; otherwise, nil.

Deprecated

### Accessing URL representations

var baseURL: URL?

The base URL.

var absoluteString: String

The absolute string for the URL.

var absoluteURL: URL

The absolute URL.

var relativePath: String

The relative path of the URL if the URL conforms to RFC 3986, otherwise nil.

var relativeString: String

The relative portion of a URL.

var standardized: URL

A version of the URL with any instances of “..” or “.” resolved in its path.

var standardizedFileURL: URL

A standardized version of the path of a file URL.

### Accessing resource values

func resourceValues(forKeys: Set&lt;URLResourceKey>) throws -> URLResourceValues

Returns a collection of resource values identified by the given resource keys.

func setResourceValues(URLResourceValues) throws

Sets the resource value identified by a given resource key.

func removeCachedResourceValue(forKey: URLResourceKey)

Removes the cached resource value identified by a given resource value key from the URL object.

func removeAllCachedResourceValues()

Removes all cached resource values and all temporary resource values from the URL object.

func setTemporaryResourceValue(any Sendable, forKey: URLResourceKey)

Sets a temporary resource value on the URL object.

struct URLResourceKey

Keys that apply to file system URLs.

struct URLResourceValues

The properties that the file system resources support.

### Working with the data representation of a URL

init?(dataRepresentation: Data, relativeTo: URL?, isAbsolute: Bool)

Initializes a newly created URL using the contents of the given data, relative to a base URL.

var dataRepresentation: Data

The data representation of the URL’s relativeString.

### Working with file URLs

var isFileURL: Bool

A Boolean that is true if the scheme is `file:`.

var hasDirectoryPath: Bool

A Boolean that is true if the URL path represents a directory.

func withUnsafeFileSystemRepresentation&lt;ResultType>((UnsafePointer&lt;Int8>?) throws -> ResultType) rethrows -> ResultType

Passes the URL’s path in the file system representation to a closure.

func resolveSymlinksInPath()

Resolves any symlinks in the path of a file URL.

func resolvingSymlinksInPath() -> URL

Resolves any symlinks in the path of a file URL.

func standardize()

Standardizes the path of a file URL.

### Accessing common directories

static var applicationDirectory: URL

The standard directory for apps.

static var applicationSupportDirectory: URL

The standard directory for application support files.

static var cachesDirectory: URL

The standard directory for discardable cache files.

static var desktopDirectory: URL

The standard directory for files on the desktop.

static var documentsDirectory: URL

The standard directory for document files.

static var downloadsDirectory: URL

The standard directory for download files.

static var libraryDirectory: URL

The standard directory for documentation, support, and configuration files.

static var moviesDirectory: URL

The standard directory for movie files.

static var musicDirectory: URL

The standard directory for music files.

static var picturesDirectory: URL

The standard directory for image files.

static var sharedPublicDirectory: URL

The standard directory for publicly shared files.

static var temporaryDirectory: URL

The standard directory for temporary files.

static var trashDirectory: URL

The standard trash directory.

static var userDirectory: URL

The container directory of user home directories.

### Accessing home and user directories

static func currentDirectory() -> URL

Returns the working directory of the current process.

static var homeDirectory: URL

The home directory for the current user.

static func homeDirectory(forUser: String) -> URL?

Returns the home directory for the specified user.

### Adding path components

func append&lt;S>(path: S, directoryHint: URL.DirectoryHint)

Appends a path to the URL, with a hint for handling directory awareness.

func append&lt;S>(component: S, directoryHint: URL.DirectoryHint)

Appends a path component to the URL, with a hint for handling directory awareness.

func appendPathComponent(String)

Appends a path component to the URL.

Deprecated

func appendPathComponent(String, isDirectory: Bool)

Appends a path component to the URL, specifying whether the resulting path is a directory.

Deprecated

func appending&lt;S>(path: S, directoryHint: URL.DirectoryHint) -> URL

Returns a URL by appending the specified path to the URL, with a hint for handling directory awareness.

func appending&lt;S>(component: S, directoryHint: URL.DirectoryHint) -> URL

Returns a URL by appending the specified path component to the URL, with a hint for handling directory awareness.

func appendingPathComponent(String) -> URL

Returns a URL by appending the specified path component to self.

Deprecated

func appendingPathComponent(String, isDirectory: Bool) -> URL

Returns a URL by appending the specified path component to self, specifying whether the resulting path is a directory.

Deprecated

func append&lt;S>(components: S..., directoryHint: URL.DirectoryHint)

Appends multiple path components to the URL, with a hint for handling directory awareness.

func appending&lt;S>(components: S..., directoryHint: URL.DirectoryHint) -> URL

Returns a new URL by appending multiple path components to the URL, with a hint for handling directory awareness.

func appendPathComponent(String, conformingTo: UTType)

Appends a path component to the URL that conforms to a uniform type identifier.

func appendingPathComponent(String, conformingTo: UTType) -> URL

Returns a URL by appending the specified path component that conforms to a uniform type identifier.

### Adding a path extension

func appendPathExtension(String)

Appends the specified path extension to self.

func appendingPathExtension(String) -> URL

Returns a URL by appending the specified path extension to self.

func appendPathExtension(for: UTType)

Appends the preferred path extension for the type you specify.

func appendingPathExtension(for: UTType) -> URL

Returns a URL by appending the preferred path extension for the type you specify to the URL’s last path component.

### Adding query items

func append(queryItems: [URLQueryItem])

Appends a list of query items to the URL.

func appending(queryItems: [URLQueryItem]) -> URL

Returns a new URL formed by appending a list of query items to the URL.

struct URLQueryItem

A single name-value pair from the query portion of a URL.

### Removing path components

func deleteLastPathComponent()

Returns a URL constructed by removing the last path component of self.

func deletingLastPathComponent() -> URL

Returns a URL constructed by removing the last path component of self.

### Removing a path extension

func deletePathExtension()

Returns a URL constructed by removing any path extension.

func deletingPathExtension() -> URL

Returns a URL constructed by removing any path extension.

### Creating bookmarks

func bookmarkData(options: URL.BookmarkCreationOptions, includingResourceValuesForKeys: Set&lt;URLResourceKey>?, relativeTo: URL?) throws -> Data

Returns bookmark data for the URL, created with specified options and resource values.

static func bookmarkData(withContentsOf: URL) throws -> Data

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

static func writeBookmarkData(Data, to: URL) throws

Creates an alias file on disk at a specified location with specified bookmark data.

static func resourceValues(forKeys: Set&lt;URLResourceKey>, fromBookmarkData: Data) -> URLResourceValues?

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

typealias BookmarkCreationOptions

An alias for bookmark creation options.

struct BookmarkCreationOptions

Options used when creating bookmark data.

### Checking reachability

func checkResourceIsReachable() throws -> Bool

Returns whether the URL’s resource exists and is reachable.

### Loading URL contents asynchronously

var resourceBytes: URL.AsyncBytes

The URL’s resource data, as an asynchronous sequence of bytes.

var lines: AsyncLineSequence&lt;URL.AsyncBytes>

The URL’s resource data, as an asynchronous sequence of lines of text.

struct AsyncBytes

An asynchronous sequence of bytes loaded from the URL.

### Working with promised items

func checkPromisedItemIsReachable() throws -> Bool

Returns whether the promised item URL’s resource exists and is reachable.

func promisedItemResourceValues(forKeys: Set&lt;URLResourceKey>) throws -> URLResourceValues

Gets resource values from URLs of ‘promised’ items.

### Working with security scoped resources

func startAccessingSecurityScopedResource() -> Bool

Given a url created by resolving a bookmark data created with security scope, make the resource referenced by the url accessible to the process.

func stopAccessingSecurityScopedResource()

Revokes the access granted to the url by a prior successful call to the complementary start function.

### Comparing URLs

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Describing a URL

var customPlaygroundQuickLook: PlaygroundQuickLook

A playground quicklook for the URL.

Deprecated

### Formatting a URL

func formatted() -> String

Formats the URL using a default format style.

func formatted&lt;F>(F) -> F.FormatOutput

Formats the URL, using the provided format style.

struct FormatStyle

A structure that converts between URL instances and their textual representations.

### Using reference types

class NSURL

An object that represents the location of a resource, such as an item on a remote server or the path to a local file.

### Core Transferable support

static var transferRepresentation: some TransferRepresentation

The representation for importing and exporting an item using Core Transferable.

typealias Representation

The data type for conformance with the Core Transferable framework.

### App Intents support

static var defaultResolverSpecification: some ResolverSpecification

The default resolver specification that the App Intents framework uses.

typealias Specification

The specification type for conforming with App Intents.

typealias UnwrappedType

The core type for conforming with App Intents.

typealias ValueType

The value type for conforming with App Intents.

### Default Implementations

CustomURLRepresentationParameterConvertible Implementations

Equatable Implementations

Transferable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- CustomURLRepresentationParameterConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- ReferenceConvertible
- Sendable
- Transferable

## See Also

### URLs

struct URLComponents

A structure that parses URLs into and constructs URLs from their constituent parts.

struct URLQueryItem

A single name-value pair from the query portion of a URL.

