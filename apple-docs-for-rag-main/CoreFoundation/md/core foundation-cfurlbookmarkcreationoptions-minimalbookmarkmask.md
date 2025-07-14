

- Core Foundation
- CFURLBookmarkCreationOptions
-  minimalBookmarkMask 

Type Property

# minimalBookmarkMask

Specifies that an alias created with the bookmark data be created with minimal information, which may make it smaller but still able to resolve in certain ways.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var minimalBookmarkMask: CFURLBookmarkCreationOptions { get }
```

## See Also

### Constants

static var preferFileIDResolutionMask: CFURLBookmarkCreationOptions

Specifies that an alias created with the bookmark data prefers resolving with its embedded file ID.

Deprecated

static var suitableForBookmarkFile: CFURLBookmarkCreationOptions

Specifies that the bookmark data include properties required to create Finder alias files.

static var withSecurityScope: CFURLBookmarkCreationOptions

Specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read/write access to a file-system resource; for use in an app that adopts App Sandbox.

static var securityScopeAllowOnlyReadAccess: CFURLBookmarkCreationOptions

When combined with the withSecurityScope option, specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read-only access to a file-system resource; for use in an app that adopts App Sandbox.

