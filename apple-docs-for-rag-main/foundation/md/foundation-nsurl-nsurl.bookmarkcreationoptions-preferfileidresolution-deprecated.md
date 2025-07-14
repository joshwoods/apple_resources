

- Foundation
- NSURL
- NSURL.BookmarkCreationOptions
-  preferFileIDResolution Deprecated

Type Property

# preferFileIDResolution

Specifies that when creating a bookmark, upon resolution, its embedded file ID takes precedence over other sources of information (file system path, for example) when there’s a conflict.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
static var preferFileIDResolution: NSURL.BookmarkCreationOptions { get }
```

Deprecated

This option does nothing and has no effect on bookmark resolution.

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

static var withoutImplicitSecurityScope: NSURL.BookmarkCreationOptions

Prevents inclusion of a bookmark’s implicit ephemeral security scope, when creating one without security scope.

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

