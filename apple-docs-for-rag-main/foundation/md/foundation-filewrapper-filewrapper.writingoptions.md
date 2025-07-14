

- Foundation
- FileWrapper
-  FileWrapper.WritingOptions 

Structure

# FileWrapper.WritingOptions

Writing options that can be set by the write(to:options:originalContentsURL:) method.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct WritingOptions
```

## Topics

### Constants

static var atomic: FileWrapper.WritingOptions

Whether writing is done atomically.

static var withNameUpdating: FileWrapper.WritingOptions

Whether descendant file wrappers’filename properties are set if the writing succeeds.

static var atomic: FileWrapper.WritingOptions

Whether writing is done atomically.

static var withNameUpdating: FileWrapper.WritingOptions

Whether descendant file wrappers’filename properties are set if the writing succeeds.

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

struct ReadingOptions

Reading options that can be set by the init(url:options:) and read(from:options:) methods.

