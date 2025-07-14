

- Foundation
- FileWrapper
-  FileWrapper.ReadingOptions 

Structure

# FileWrapper.ReadingOptions

Reading options that can be set by the init(url:options:) and read(from:options:) methods.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct ReadingOptions
```

## Overview

You can use the `NSFileWrapperReadingImmediate` and `NSFileWrapperReadingWithoutMapping` reading options together to take an exact snapshot of a file-system hierarchy that is safe from all errors (including the ones mentioned above) once reading has succeeded. If reading with both options succeeds, then subsequent invocations of the methods listed in the comment for the `NSFileWrapperReadingImmediate` reading option to the receiver and all its descendant file wrappers will never fail. However, note that reading with both options together is expensive in terms of both I/O and memory for large files, or directories containing large files, or even directories containing many small files.

## Topics

### Constants

static var immediate: FileWrapper.ReadingOptions

The option to read files immediately after creating a file wrapper.

static var withoutMapping: FileWrapper.ReadingOptions

Whether file mapping for regular file wrappers is disallowed.

static var immediate: FileWrapper.ReadingOptions

The option to read files immediately after creating a file wrapper.

static var withoutMapping: FileWrapper.ReadingOptions

Whether file mapping for regular file wrappers is disallowed.

### Initializers

init(rawValue: UInt)

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

Writing options that can be set by the write(to:options:originalContentsURL:) method.

