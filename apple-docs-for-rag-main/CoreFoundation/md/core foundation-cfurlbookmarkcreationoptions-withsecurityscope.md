

- Core Foundation
- CFURLBookmarkCreationOptions
-  withSecurityScope 

Type Property

# withSecurityScope

Specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read/write access to a file-system resource; for use in an app that adopts App Sandbox.

Mac Catalyst 13.0+macOS 10.7+

``` source
static var withSecurityScope: CFURLBookmarkCreationOptions { get }
```

## See Also

### Constants

static var preferFileIDResolutionMask: CFURLBookmarkCreationOptions

Specifies that an alias created with the bookmark data prefers resolving with its embedded file ID.

Deprecated

static var minimalBookmarkMask: CFURLBookmarkCreationOptions

Specifies that an alias created with the bookmark data be created with minimal information, which may make it smaller but still able to resolve in certain ways.

static var suitableForBookmarkFile: CFURLBookmarkCreationOptions

Specifies that the bookmark data include properties required to create Finder alias files.

static var securityScopeAllowOnlyReadAccess: CFURLBookmarkCreationOptions

When combined with the withSecurityScope option, specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read-only access to a file-system resource; for use in an app that adopts App Sandbox.

