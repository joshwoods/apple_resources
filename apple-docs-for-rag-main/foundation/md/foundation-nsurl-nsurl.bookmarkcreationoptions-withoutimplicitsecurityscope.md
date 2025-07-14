

- Foundation
- NSURL
- NSURL.BookmarkCreationOptions
-  withoutImplicitSecurityScope 

Type Property

# withoutImplicitSecurityScope

Prevents inclusion of a bookmark’s implicit ephemeral security scope, when creating one without security scope.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var withoutImplicitSecurityScope: NSURL.BookmarkCreationOptions { get }
```

## Discussion

Bookmarks that you create without security scope automatically carry implicit ephemeral security scope. This security scope is valid until reboot at the latest, and confers access to the resource to any other process that resolves the bookmark. Using this option prevents inclusion of this ephemeral security scope.

When using this option, other processes can’t call startAccessingSecurityScopedResource() on the resolved URL. The option prevents providing unintended access to resources to other processes, and is also a performance optimization that reduces the size of the bookmark.

## See Also

### Options

static var minimalBookmark: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, it includes minimal information.

static var suitableForBookmarkFile: NSURL.BookmarkCreationOptions

Specifies that the bookmark data includes the required properties for creating Finder alias files.

static var withSecurityScope: NSURL.BookmarkCreationOptions

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read/write access to a file-system resource.

static var securityScopeAllowOnlyReadAccess: NSURL.BookmarkCreationOptions

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read-only access to a file-system resource.

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

static var preferFileIDResolution: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, upon resolution, its embedded file ID takes precedence over other sources of information (file system path, for example) when there’s a conflict.

Deprecated

