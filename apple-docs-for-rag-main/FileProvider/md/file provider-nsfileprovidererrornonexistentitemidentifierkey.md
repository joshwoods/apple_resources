

- File Provider
-  NSFileProviderErrorNonExistentItemIdentifierKey 

Global Variable

# NSFileProviderErrorNonExistentItemIdentifierKey

The key for accessing the specified item’s identifier when the item doesn’t exist.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
let NSFileProviderErrorNonExistentItemIdentifierKey: String
```

## Discussion

Use this key to access the item’s identifier from a noSuchItem error’s userInfo dictionary.

## See Also

### Errors

struct NSFileProviderError

A structure that contains information about File Provider extension errors.

enum Code

The error codes for the File Provider extension.

let NSFileProviderErrorDomain: String

The error domain for the File Provider extension.

let NSFileProviderErrorItemKey: String

The key for accessing information about sync-related errors.

let NSFileProviderErrorCollidingItemKey: String

The key for accessing the existing item from a filename collision error’s user info dictionary.

Deprecated

