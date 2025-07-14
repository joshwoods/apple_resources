

- Foundation
- FileManager
- FileManager.ItemReplacementOptions
-  init(rawValue:) 

Initializer

# init(rawValue:)

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(rawValue: UInt)
```

## See Also

### Using File Replacement Options

static var usingNewMetadataOnly: FileManager.ItemReplacementOptions

Only metadata from the new item is used, and metadata from the original item isn’t preserved (default).

static var withoutDeletingBackupItem: FileManager.ItemReplacementOptions

The backup item remains in place after a successful replacement.

