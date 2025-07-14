

- Foundation
- NSFileCoordinator
-  NSFileCoordinator.WritingOptions 

Structure

# NSFileCoordinator.WritingOptions

Options to use when changing the contents or attributes of a file or directory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct WritingOptions
```

## Overview

You must specify only one constant at a time for a given write operation.

## Topics

### Constants

static var forDeleting: NSFileCoordinator.WritingOptions

static var forMoving: NSFileCoordinator.WritingOptions

static var forMerging: NSFileCoordinator.WritingOptions

static var forReplacing: NSFileCoordinator.WritingOptions

static var contentIndependentMetadataOnly: NSFileCoordinator.WritingOptions

Select this option when writing to change the file’s metadata only and not its contents.

### Createing a Writing Option

init(rawValue: UInt)

static var forDeleting: NSFileCoordinator.WritingOptions

static var forMoving: NSFileCoordinator.WritingOptions

static var forMerging: NSFileCoordinator.WritingOptions

static var forReplacing: NSFileCoordinator.WritingOptions

static var contentIndependentMetadataOnly: NSFileCoordinator.WritingOptions

Select this option when writing to change the file’s metadata only and not its contents.

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

struct ReadingOptions

Options to use when reading the contents or attributes of a file or directory.

