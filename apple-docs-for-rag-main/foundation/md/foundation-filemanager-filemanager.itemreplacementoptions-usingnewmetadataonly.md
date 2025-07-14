

- Foundation
- FileManager
- FileManager.ItemReplacementOptions
-  usingNewMetadataOnly 

Type Property

# usingNewMetadataOnly

Only metadata from the new item is used, and metadata from the original item isn’t preserved (default).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var usingNewMetadataOnly: FileManager.ItemReplacementOptions { get }
```

## See Also

### Using File Replacement Options

init(rawValue: UInt)

static var withoutDeletingBackupItem: FileManager.ItemReplacementOptions

The backup item remains in place after a successful replacement.

