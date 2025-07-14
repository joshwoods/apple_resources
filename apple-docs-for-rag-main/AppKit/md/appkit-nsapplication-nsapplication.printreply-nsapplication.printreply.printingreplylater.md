

- AppKit
- NSApplication
- NSApplication.PrintReply
-  NSApplication.PrintReply.printingReplyLater 

Case

# NSApplication.PrintReply.printingReplyLater

macOS

``` source
case printingReplyLater
```

## Discussion

The result of printing cannot be returned immediately, for example, if printing will cause the presentation of a sheet. If your method returns `NSPrintingReplyLater` it must always invoke reply(toOpenOrPrint:) when the entire print operation has been completed, successfully or not.

## See Also

### Constants

case printingCancelled

Printing was cancelled.

case printingSuccess

Printing was successful.

case printingFailure

Printing failed.

