

- AppKit
- NSPrintInfo
-  NSPrintInfo.SettingKey 

Type Alias

# NSPrintInfo.SettingKey

The type you use to specify a print info setting key.

macOS

``` source
typealias SettingKey = String
```

## See Also

### Accessing Core Printing Information

var printSettings: NSMutableDictionary

A mutable dictionary containing the print settings from Core Printing.

func pmPrintSession() -> UnsafeMutableRawPointer

Returns a Core Printing object configured with the print info’s session information.

func pmPageFormat() -> UnsafeMutableRawPointer

Returns a Core Printing object configured with the print info’s page format information.

func pmPrintSettings() -> UnsafeMutableRawPointer

Returns a Core Printing object configured with the print info’s print settings information

func updateFromPMPageFormat()

Synchronizes the print info’s page format information with information from its associated page format object.

func updateFromPMPrintSettings()

Synchronizes the print info’s print settings information with information from its associated print settings object.

func takeSettings(from: NSPDFInfo)

Updates the print info with all the settings and attributes in the specified PDF info object.

