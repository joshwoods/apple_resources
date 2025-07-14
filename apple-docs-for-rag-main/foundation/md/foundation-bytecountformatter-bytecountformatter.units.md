

- Foundation
- ByteCountFormatter
-  ByteCountFormatter.Units 

Structure

# ByteCountFormatter.Units

Specifies the units appropriate for the formatter to display. Specifying any units explicitly causes just those units to be used in showing the number.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Units
```

## Topics

### Constants

static var useBytes: ByteCountFormatter.Units

Displays bytes in the formatter content.

static var useKB: ByteCountFormatter.Units

Displays kilobytes in the formatter content.

static var useMB: ByteCountFormatter.Units

Displays megabytes in the formatter content.

static var useGB: ByteCountFormatter.Units

Displays gigabytes in the formatter content.

static var useTB: ByteCountFormatter.Units

Displays terabytes in the formatter content.

static var usePB: ByteCountFormatter.Units

Displays petabyte in the formatter content.

static var useEB: ByteCountFormatter.Units

Displays exabytes in the formatter content.

static var useZB: ByteCountFormatter.Units

Displays zettabytes in the formatter content.

static var useYBOrHigher: ByteCountFormatter.Units

Displays yottabytes in the formatter content.

static var useAll: ByteCountFormatter.Units

Can use any unit in the formatter content.

static var useBytes: ByteCountFormatter.Units

Displays bytes in the formatter content.

static var useKB: ByteCountFormatter.Units

Displays kilobytes in the formatter content.

static var useMB: ByteCountFormatter.Units

Displays megabytes in the formatter content.

static var useGB: ByteCountFormatter.Units

Displays gigabytes in the formatter content.

static var useTB: ByteCountFormatter.Units

Displays terabytes in the formatter content.

static var usePB: ByteCountFormatter.Units

Displays petabyte in the formatter content.

static var useEB: ByteCountFormatter.Units

Displays exabytes in the formatter content.

static var useZB: ByteCountFormatter.Units

Displays zettabytes in the formatter content.

static var useYBOrHigher: ByteCountFormatter.Units

Displays yottabytes in the formatter content.

static var useAll: ByteCountFormatter.Units

Can use any unit in the formatter content.

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

enum CountStyle

Specifies display of file or storage byte counts. The display style is platform specific.

