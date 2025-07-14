

- AppKit
- NSPrintInfo
-  updateFromPMPageFormat() 

Instance Method

# updateFromPMPageFormat()

Synchronizes the print info’s page format information with information from its associated page format object.

macOS 10.5+

``` source
func updateFromPMPageFormat()
```

## Discussion

You should use this method after making changes to the `PMPageFormat` object obtained from the receiver. Each `NSPrintInfo` object keeps track of the object returned from its pmPageFormat() method and obtains any updated information from the object directly. You only need to synchronize the objects once when you have made all of the desired changes.

## See Also

### Accessing Core Printing Information

var printSettings: NSMutableDictionary

A mutable dictionary containing the print settings from Core Printing.

typealias SettingKey

The type you use to specify a print info setting key.

func pmPrintSession() -> UnsafeMutableRawPointer

Returns a Core Printing object configured with the print info’s session information.

func pmPageFormat() -> UnsafeMutableRawPointer

Returns a Core Printing object configured with the print info’s page format information.

func pmPrintSettings() -> UnsafeMutableRawPointer

Returns a Core Printing object configured with the print info’s print settings information

func updateFromPMPrintSettings()

Synchronizes the print info’s print settings information with information from its associated print settings object.

func takeSettings(from: NSPDFInfo)

Updates the print info with all the settings and attributes in the specified PDF info object.

