

- Core Spotlight
-  CSIndexExtensionRequestHandler 

Class

# CSIndexExtensionRequestHandler

An interface that implements an index-maintenance app extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class CSIndexExtensionRequestHandler
```

## Overview

The `CSIndexExtensionRequestHandler` class provides the main entry point for an index-maintenance app extension. If any issues arise with your app’s indexes and your app isn’t running, the system loads your app extension and looks for an implementation of this class. It instantiates the class it finds and uses it to perform any index-related maintenance.

Define a custom subclass of `CSIndexExtensionRequestHandler` in your app extension and implement methods of the CSSearchableIndexDelegate protocol in it. Use those methods to perform any required updates to your app’s index files. For example, use the searchableIndex(_:reindexAllSearchableItemsWithAcknowledgementHandler:) method to reindex all items in your app.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CSSearchableIndexDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSExtensionRequestHandling
- NSObjectProtocol

## See Also

### Spotlight app extensions

Regenerating your app’s indexes on demand

Create an app extension to maintain your app’s indexes and regenerate them as needed.

class CSImportExtension

An object that provides searchable attributes for file types that the app supports.

