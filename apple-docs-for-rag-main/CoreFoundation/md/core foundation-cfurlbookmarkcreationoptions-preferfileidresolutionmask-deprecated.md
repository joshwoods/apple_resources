

- Core Foundation
- CFURLBookmarkCreationOptions
-  preferFileIDResolutionMask Deprecated

Type Property

# preferFileIDResolutionMask

Specifies that an alias created with the bookmark data prefers resolving with its embedded file ID.

tvOS 9.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
static var preferFileIDResolutionMask: CFURLBookmarkCreationOptions { get }
```

Deprecated

kCFURLBookmarkCreationPreferFileIDResolutionMask does nothing and has no effect on bookmark resolution

## See Also

### Constants

static var minimalBookmarkMask: CFURLBookmarkCreationOptions

Specifies that an alias created with the bookmark data be created with minimal information, which may make it smaller but still able to resolve in certain ways.

static var suitableForBookmarkFile: CFURLBookmarkCreationOptions

Specifies that the bookmark data include properties required to create Finder alias files.

static var withSecurityScope: CFURLBookmarkCreationOptions

Specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read/write access to a file-system resource; for use in an app that adopts App Sandbox.

static var securityScopeAllowOnlyReadAccess: CFURLBookmarkCreationOptions

When combined with the withSecurityScope option, specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read-only access to a file-system resource; for use in an app that adopts App Sandbox.

