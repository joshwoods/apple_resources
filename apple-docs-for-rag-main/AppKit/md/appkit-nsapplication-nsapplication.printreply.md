

- AppKit
- NSApplication
-  NSApplication.PrintReply 

Enumeration

# NSApplication.PrintReply

Constants that indicate the outcome of a print request.

macOS

``` source
enum PrintReply
```

## Topics

### Constants

case printingCancelled

Printing was cancelled.

case printingSuccess

Printing was successful.

case printingFailure

Printing failed.

case printingReplyLater

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Printing

func application(NSApplication, printFile: String) -> Bool

Returns a Boolean value that indicates if the app prints the specified file in its entirety.

func application(NSApplication, printFiles: [String], withSettings: [NSPrintInfo.AttributeKey : Any], showPrintPanels: Bool) -> NSApplication.PrintReply

Returns a value that indicates if the app prints the specified files.

