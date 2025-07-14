

- Application Services
- ApplicationServices Functions
-  PMPrinterSendCommand(\_:\_:\_:\_:) 

Function

# PMPrinterSendCommand(\_:\_:\_:\_:)

macOS 10.6+

``` source
func PMPrinterSendCommand(
    _ printer: PMPrinter,
    _ commandString: CFString,
    _ jobTitle: CFString?,
    _ options: CFDictionary?
) -> OSStatus
```

