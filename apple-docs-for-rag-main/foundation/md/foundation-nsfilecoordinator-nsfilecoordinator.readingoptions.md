

- Foundation
- NSFileCoordinator
-  NSFileCoordinator.ReadingOptions 

Structure

# NSFileCoordinator.ReadingOptions

Options to use when reading the contents or attributes of a file or directory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct ReadingOptions
```

## Topics

### Constants

static var withoutChanges: NSFileCoordinator.ReadingOptions

static var resolvesSymbolicLink: NSFileCoordinator.ReadingOptions

static var immediatelyAvailableMetadataOnly: NSFileCoordinator.ReadingOptions

Specify this constant if you want to read an item’s metadata without triggering a download.

static var forUploading: NSFileCoordinator.ReadingOptions

Specify this content when reading an item for the purpose of uploading its contents.

### Creating a Reading Option

init(rawValue: UInt)

static var withoutChanges: NSFileCoordinator.ReadingOptions

static var resolvesSymbolicLink: NSFileCoordinator.ReadingOptions

static var immediatelyAvailableMetadataOnly: NSFileCoordinator.ReadingOptions

Specify this constant if you want to read an item’s metadata without triggering a download.

static var forUploading: NSFileCoordinator.ReadingOptions

Specify this content when reading an item for the purpose of uploading its contents.

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

### Constants

struct WritingOptions

Options to use when changing the contents or attributes of a file or directory.

