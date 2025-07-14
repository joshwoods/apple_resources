

- AppKit
- NSPrintInfo
-  pmPrintSession() 

Instance Method

# pmPrintSession()

Returns a Core Printing object configured with the print info’s session information.

macOS 10.5+

``` source
func pmPrintSession() -> UnsafeMutableRawPointer
```

## Return Value

A pointer to a PMPrintSession object, an opaque type that stores information about a print job. You should not call `PMRelease` to release the returned object, except to balance calls to `PMRetain` that your code also issued.

## Discussion

The information in the returned `PMPrintSession` object is consistent with the receiver’s session information at the time this method is called. Subsequent changes to the receiving `NSPrintInfo` object do not result in changes to the information in the `PMPrintSession` object.

## See Also

### Accessing Core Printing Information

var printSettings: NSMutableDictionary

A mutable dictionary containing the print settings from Core Printing.

typealias SettingKey

The type you use to specify a print info setting key.

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

