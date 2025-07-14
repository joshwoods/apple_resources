

- Foundation
- NSURL
-  NSURL.BookmarkCreationOptions 

Structure

# NSURL.BookmarkCreationOptions

Options used when creating bookmark data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct BookmarkCreationOptions
```

## Overview

When creating a bookmark, use bitwise `OR` operators to combine the options you want to specify, and provide them to the `options` parameter of the bookmarkData(options:includingResourceValuesForKeys:relativeTo:) method.

Note

Security-scoped bookmarks aren’t available in versions of macOS prior to 10.7.3.

## Topics

### Creating a bookmark creation option

init(rawValue: UInt)

### Options

static var minimalBookmark: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, it includes minimal information.

static var suitableForBookmarkFile: NSURL.BookmarkCreationOptions

Specifies that the bookmark data includes the required properties for creating Finder alias files.

static var withSecurityScope: NSURL.BookmarkCreationOptions

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read/write access to a file-system resource.

static var securityScopeAllowOnlyReadAccess: NSURL.BookmarkCreationOptions

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read-only access to a file-system resource.

static var withoutImplicitSecurityScope: NSURL.BookmarkCreationOptions

Prevents inclusion of a bookmark’s implicit ephemeral security scope, when creating one without security scope.

static var preferFileIDResolution: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, upon resolution, its embedded file ID takes precedence over other sources of information (file system path, for example) when there’s a conflict.

Deprecated

static var minimalBookmark: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, it includes minimal information.

static var suitableForBookmarkFile: NSURL.BookmarkCreationOptions

Specifies that the bookmark data includes the required properties for creating Finder alias files.

static var withSecurityScope: NSURL.BookmarkCreationOptions

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read/write access to a file-system resource.

static var securityScopeAllowOnlyReadAccess: NSURL.BookmarkCreationOptions

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read-only access to a file-system resource.

static var withoutImplicitSecurityScope: NSURL.BookmarkCreationOptions

Prevents inclusion of a bookmark’s implicit ephemeral security scope, when creating one without security scope.

static var preferFileIDResolution: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, upon resolution, its embedded file ID takes precedence over other sources of information (file system path, for example) when there’s a conflict.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

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

struct BookmarkResolutionOptions

Options used when resolving bookmark data.

