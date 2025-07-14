

- Foundation
- NSURL
- NSURL.BookmarkCreationOptions
-  suitableForBookmarkFile 

Type Property

# suitableForBookmarkFile

Specifies that the bookmark data includes the required properties for creating Finder alias files.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var suitableForBookmarkFile: NSURL.BookmarkCreationOptions { get }
```

## See Also

### Options

static var minimalBookmark: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, it includes minimal information.

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

static var withSecurityScope: NSURL.BookmarkCreationOptions

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read/write access to a file-system resource.

static var securityScopeAllowOnlyReadAccess: NSURL.BookmarkCreationOptions

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read-only access to a file-system resource.

static var withoutImplicitSecurityScope: NSURL.BookmarkCreationOptions

Prevents inclusion of a bookmark’s implicit ephemeral security scope, when creating one without security scope.

static var preferFileIDResolution: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, upon resolution, its embedded file ID takes precedence over other sources of information (file system path, for example) when there’s a conflict.

Deprecated

