

- Application Services
- Core Printing
-  PMSetDuplex(\_:\_:) 

Function

# PMSetDuplex(\_:\_:)

Sets the duplex mode.

macOS 10.4+

``` source
func PMSetDuplex(
    _ printSettings: PMPrintSettings,
    _ duplexSetting: PMDuplexMode
) -> OSStatus
```

## Parameters 

`printSettings`  

The print settings object whose duplex mode you want to set.

`duplexSetting`  

The new duplex mode setting. Possible values include:

- `kPMDuplexNone` (one-sided printing)

- `kPMDuplexNoTumble` (two-sided printing)

- `kPMDuplexTumble` (two-sided printing with tumbling)

See PMDuplexMode for a full description of the constants you can use to specify the new setting.

## Return Value

A result code. See Result Codes.

## Discussion

Duplex printing is a print job that prints on both sides of the paper. Two-Sided printing controls are displayed in the Layout pane of the Print dialog. This function allows you to specify whether the document should be printed single-sided, double-sided with short-edge binding, or double-sided with long-edge binding.

Note

Not all printers support duplex printing. This function specifies a setting that might not be available on a given destination.

If you call this function after initiating a print job, the change is ignored for the current job.

## See Also

### Accessing Data in Print Settings Objects

func PMGetFirstPage(PMPrintSettings, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Obtains the number of the first page to be printed.

func PMSetFirstPage(PMPrintSettings, UInt32, Bool) -> OSStatus

Sets the default page number of the first page to be printed.

func PMGetLastPage(PMPrintSettings, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Obtains the number of the last page to be printed.

func PMSetLastPage(PMPrintSettings, UInt32, Bool) -> OSStatus

Sets the page number of the last page to be printed.

func PMGetPageRange(PMPrintSettings, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Obtains the valid range of pages that can be printed.

func PMSetPageRange(PMPrintSettings, UInt32, UInt32) -> OSStatus

Sets the valid range of pages that can be printed.

func PMPrintSettingsGetJobName(PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Obtains the name of a print job.

func PMPrintSettingsSetJobName(PMPrintSettings, CFString) -> OSStatus

Specifies the name of a print job.

func PMGetCopies(PMPrintSettings, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Obtains the number of copies that the user requests to be printed.

func PMSetCopies(PMPrintSettings, UInt32, Bool) -> OSStatus

Sets the initial value for the number of copies to be printed.

func PMGetCollate(PMPrintSettings, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Obtains a Boolean value that indicates whether the job collate option is selected.

func PMSetCollate(PMPrintSettings, Bool) -> OSStatus

Specifies whether the job collate option is selected.

func PMGetDuplex(PMPrintSettings, UnsafeMutablePointer&lt;PMDuplexMode>) -> OSStatus

Obtains the selected duplex mode.

func PMPrintSettingsGetValue(PMPrintSettings, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFTypeRef>?>) -> OSStatus

Obtains the value of a setting in a print settings object.

func PMPrintSettingsSetValue(PMPrintSettings, CFString, CFTypeRef?, Bool) -> OSStatus

Stores the value of a setting in a print settings object.

func PMPrintSettingsCopyAsDictionary(PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

Creates a dictionary that contains the settings in a print settings object.

func PMPrintSettingsCopyKeys(PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains the keys for items in a print settings object.

