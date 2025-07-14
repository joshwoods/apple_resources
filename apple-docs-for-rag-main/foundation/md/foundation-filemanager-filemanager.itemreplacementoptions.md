

- Foundation
- FileManager
-  FileManager.ItemReplacementOptions 

Structure

# FileManager.ItemReplacementOptions

Options for specifying the behavior of file replacement operations.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct ItemReplacementOptions
```

## Overview

These options are used by replaceItem(at:withItemAt:backupItemName:options:resultingItemURL:).

## Topics

### Using File Replacement Options

init(rawValue: UInt)

static var usingNewMetadataOnly: FileManager.ItemReplacementOptions

Only metadata from the new item is used, and metadata from the original item isn’t preserved (default).

static var withoutDeletingBackupItem: FileManager.ItemReplacementOptions

The backup item remains in place after a successful replacement.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Replacing Items

func replaceItemAt(URL, withItemAt: URL, backupItemName: String?, options: FileManager.ItemReplacementOptions) throws -> URL?

Replaces the contents of the item at the specified URL in a manner that ensures no data loss occurs.

func replaceItem(at: URL, withItemAt: URL, backupItemName: String?, options: FileManager.ItemReplacementOptions, resultingItemURL: AutoreleasingUnsafeMutablePointer&lt;NSURL?>?) throws

Replaces the contents of the item at the specified URL in a manner that ensures no data loss occurs.

