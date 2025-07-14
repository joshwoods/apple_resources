

- Foundation
- NSURL
-  NSURL.BookmarkResolutionOptions 

Structure

# NSURL.BookmarkResolutionOptions

Options used when resolving bookmark data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct BookmarkResolutionOptions
```

## Overview

When resolving a bookmark, use bitwise `OR` operators to combine the options you want to specify, and provide them to the `options` parameter of the URLByResolvingBookmarkData:options:relativeToURL:bookmarkDataIsStale:error: method.

### Version-Notes

Security-scoped bookmarks are not available in versions of macOS prior to OS X 10.7.3.

## Topics

### Initializers

init(rawValue: UInt)

### Constants

static var withoutUI: NSURL.BookmarkResolutionOptions

Specifies that no UI feedback should accompany resolution of the bookmark data.

static var withoutMounting: NSURL.BookmarkResolutionOptions

Specifies that no volume should be mounted during resolution of the bookmark data.

static var withSecurityScope: NSURL.BookmarkResolutionOptions

Specifies that the security scope, applied to the bookmark when it was created, should be used during resolution of the bookmark data.

static var withoutImplicitStartAccessing: NSURL.BookmarkResolutionOptions

A property that specifies that resolution doesn’t implicitly start accessing the ephemeral security-scoped resource.

static var withoutUI: NSURL.BookmarkResolutionOptions

Specifies that no UI feedback should accompany resolution of the bookmark data.

static var withoutMounting: NSURL.BookmarkResolutionOptions

Specifies that no volume should be mounted during resolution of the bookmark data.

static var withSecurityScope: NSURL.BookmarkResolutionOptions

Specifies that the security scope, applied to the bookmark when it was created, should be used during resolution of the bookmark data.

static var withoutImplicitStartAccessing: NSURL.BookmarkResolutionOptions

A property that specifies that resolution doesn’t implicitly start accessing the ephemeral security-scoped resource.

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

struct BookmarkCreationOptions

Options used when creating bookmark data.

