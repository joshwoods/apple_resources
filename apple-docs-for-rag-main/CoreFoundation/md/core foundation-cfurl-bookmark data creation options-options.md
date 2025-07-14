

- Core Foundation
- CFURL
-  Bookmark Data Creation Options 

API Collection

# Bookmark Data Creation Options

Options used when creating bookmark data.

## Overview

When creating a bookmark, use bitwise `OR` operators to combine the options you want to specify, and provide them to the `options` parameter of the CFURLCreateBookmarkData(_:_:_:_:_:_:) method.

### Version-Notes

Security-scoped bookmarks are not available in versions of macOS prior to OS X v10.7.3.

## Topics

### Constants

static var preferFileIDResolutionMask: CFURLBookmarkCreationOptions

Specifies that an alias created with the bookmark data prefers resolving with its embedded file ID.

Deprecated

static var minimalBookmarkMask: CFURLBookmarkCreationOptions

Specifies that an alias created with the bookmark data be created with minimal information, which may make it smaller but still able to resolve in certain ways.

static var suitableForBookmarkFile: CFURLBookmarkCreationOptions

Specifies that the bookmark data include properties required to create Finder alias files.

static var withSecurityScope: CFURLBookmarkCreationOptions

Specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read/write access to a file-system resource; for use in an app that adopts App Sandbox.

static var securityScopeAllowOnlyReadAccess: CFURLBookmarkCreationOptions

When combined with the withSecurityScope option, specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read-only access to a file-system resource; for use in an app that adopts App Sandbox.

## See Also

### Bookmark Data Constants

Bookmark Data Resolution Options

Options used when resolving bookmark data.

