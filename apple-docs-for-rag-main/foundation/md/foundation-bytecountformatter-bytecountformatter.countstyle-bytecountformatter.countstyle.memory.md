

- Foundation
- ByteCountFormatter
- ByteCountFormatter.CountStyle
-  ByteCountFormatter.CountStyle.memory 

Case

# ByteCountFormatter.CountStyle.memory

Specifies display of memory byte counts. The actual behavior for this is platform-specific; in macOS 10.8, this uses the binary style, but that may change over time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case memory
```

## See Also

### Constants

case file

Specifies display of file byte counts. The actual behavior for this is platform-specific; in macOS 10.8, this uses the decimal style, but that may change over time.

case decimal

Causes 1000 bytes to be shown as 1 KB. It is better to use ByteCountFormatter.CountStyle.file or ByteCountFormatter.CountStyle.memory in most cases.

case binary

Causes 1024 bytes to be shown as 1 KB. It is better to use ByteCountFormatter.CountStyle.file or ByteCountFormatter.CountStyle.memory in most cases.

case file

Specifies display of file byte counts. The actual behavior for this is platform-specific; in macOS 10.8, this uses the decimal style, but that may change over time.

case decimal

Causes 1000 bytes to be shown as 1 KB. It is better to use ByteCountFormatter.CountStyle.file or ByteCountFormatter.CountStyle.memory in most cases.

case binary

Causes 1024 bytes to be shown as 1 KB. It is better to use ByteCountFormatter.CountStyle.file or ByteCountFormatter.CountStyle.memory in most cases.

