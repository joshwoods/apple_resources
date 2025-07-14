

- File Provider
-  NSFileProviderErrorItemKey 

Global Variable

# NSFileProviderErrorItemKey

The key for accessing information about sync-related errors.

iOS 13.0+iPadOS 13.0+macOS 10.15+visionOS 1.0+

``` source
let NSFileProviderErrorItemKey: String
```

## Discussion

If a specific item caused the error, the system sets the NSFileProviderErrorItemKey key to the item’s identifier, and it sets the NSUnderlyingErrorKey key to the error encountered by the item.

## See Also

### Errors

struct NSFileProviderError

A structure that contains information about File Provider extension errors.

enum Code

The error codes for the File Provider extension.

let NSFileProviderErrorDomain: String

The error domain for the File Provider extension.

let NSFileProviderErrorNonExistentItemIdentifierKey: String

The key for accessing the specified item’s identifier when the item doesn’t exist.

let NSFileProviderErrorCollidingItemKey: String

The key for accessing the existing item from a filename collision error’s user info dictionary.

Deprecated

