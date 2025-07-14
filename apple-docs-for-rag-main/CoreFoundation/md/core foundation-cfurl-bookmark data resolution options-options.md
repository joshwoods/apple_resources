

- Core Foundation
- CFURL
-  Bookmark Data Resolution Options 

API Collection

# Bookmark Data Resolution Options

Options used when resolving bookmark data.

## Overview

When resolving a bookmark to obtain a URL, use bitwise `OR` operators to combine the options you want to specify, and provide them to the `options` parameter of the CFURLCreateByResolvingBookmarkData(_:_:_:_:_:_:_:) function.

### Version-Notes

Security-scoped bookmarks are not available in versions of macOS prior to OS X v10.7.3.

## Topics

### Constants

static var cfBookmarkResolutionWithoutUIMask: CFURLBookmarkResolutionOptions

Specifies that no UI feedback accompany resolution of the bookmark data.

static var cfBookmarkResolutionWithoutMountingMask: CFURLBookmarkResolutionOptions

Specifies that no volume should be mounted during resolution of the bookmark data.

static var cfurlBookmarkResolutionWithSecurityScope: CFURLBookmarkResolutionOptions

Specifies that the security scope, applied to the bookmark when it was created, should be used during resolution of the bookmark data.

## See Also

### Bookmark Data Constants

Bookmark Data Creation Options

Options used when creating bookmark data.

