

- Foundation
- NSURL
- NSURL.BookmarkCreationOptions
-  securityScopeAllowOnlyReadAccess 

Type Property

# securityScopeAllowOnlyReadAccess

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read-only access to a file-system resource.

macOS 10.7+

``` source
static var securityScopeAllowOnlyReadAccess: NSURL.BookmarkCreationOptions { get }
```

## Discussion

This option is only meaningful when used along with the withSecurityScope option,

Use this option in an app that adopts App Sandbox. For more information, see App Sandbox Design Guide.

## See Also

### Options

static var minimalBookmark: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, it includes minimal information.

static var suitableForBookmarkFile: NSURL.BookmarkCreationOptions

Specifies that the bookmark data includes the required properties for creating Finder alias files.

static var withSecurityScope: NSURL.BookmarkCreationOptions

Specifies that when creating a security-scoped bookmark, upon resolution, it provides a security-scoped URL allowing read/write access to a file-system resource.

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

static var withoutImplicitSecurityScope: NSURL.BookmarkCreationOptions

Prevents inclusion of a bookmark’s implicit ephemeral security scope, when creating one without security scope.

static var preferFileIDResolution: NSURL.BookmarkCreationOptions

Specifies that when creating a bookmark, upon resolution, its embedded file ID takes precedence over other sources of information (file system path, for example) when there’s a conflict.

Deprecated

