

- Foundation
- ByteCountFormatter
-  ByteCountFormatter.CountStyle 

Enumeration

# ByteCountFormatter.CountStyle

Specifies display of file or storage byte counts. The display style is platform specific.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CountStyle
```

## Topics

### Constants

case file

Specifies display of file byte counts. The actual behavior for this is platform-specific; in macOS 10.8, this uses the decimal style, but that may change over time.

case memory

Specifies display of memory byte counts. The actual behavior for this is platform-specific; in macOS 10.8, this uses the binary style, but that may change over time.

case decimal

Causes 1000 bytes to be shown as 1 KB. It is better to use ByteCountFormatter.CountStyle.file or ByteCountFormatter.CountStyle.memory in most cases.

case binary

Causes 1024 bytes to be shown as 1 KB. It is better to use ByteCountFormatter.CountStyle.file or ByteCountFormatter.CountStyle.memory in most cases.

case file

Specifies display of file byte counts. The actual behavior for this is platform-specific; in macOS 10.8, this uses the decimal style, but that may change over time.

case memory

Specifies display of memory byte counts. The actual behavior for this is platform-specific; in macOS 10.8, this uses the binary style, but that may change over time.

case decimal

Causes 1000 bytes to be shown as 1 KB. It is better to use ByteCountFormatter.CountStyle.file or ByteCountFormatter.CountStyle.memory in most cases.

case binary

Causes 1024 bytes to be shown as 1 KB. It is better to use ByteCountFormatter.CountStyle.file or ByteCountFormatter.CountStyle.memory in most cases.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct Units

Specifies the units appropriate for the formatter to display. Specifying any units explicitly causes just those units to be used in showing the number.

