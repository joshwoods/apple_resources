

- Finder Sync
-  FIFinderSyncController 

Class

# FIFinderSyncController

A controller that acts as a bridge between your Finder Sync extension and the Finder itself.

macOS 10.10+

``` source
class FIFinderSyncController
```

## Overview

Use the Finder Sync controller to configure your extension, to set badges on items in the Finder’s window, and to get a list of selected and targeted items.

## Topics

### Managing the Finder Sync Controller

class func `default`() -> Self

Returns the shared Finder Sync controller object.

var directoryURLs: Set&lt;URL>!

The directories managed by this extension.

func selectedItemURLs() -> [URL]?

Returns an array of selected items.

func setBadgeIdentifier(String, for: URL)

Sets the badge for a file or directory.

func setBadgeImage(NSImage, label: String?, forBadgeIdentifier: String)

Sets the badge image and label for the given ID.

func targetedURL() -> URL?

Returns the URL of the Finder’s current target.

### Instance Methods

func lastUsedDateForItem(with: URL) -> Date?

func setLastUsedDate(Date, forItemWith: URL, completion: (any Error) -> Void)

func setTagData(Data?, forItemWith: URL, completion: (any Error) -> Void)

func tagDataForItem(with: URL) -> Data?

### Type Properties

class var isExtensionEnabled: Bool

### Type Methods

class func showExtensionManagementInterface()

## Relationships

### Inherits From

- NSExtensionContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

class FIFinderSync

A type to subclass to add badges, custom shortcut menus, and toolbar buttons to the Finder.

