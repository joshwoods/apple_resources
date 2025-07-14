

- Application Services
- Core Printing
-  PMPrintSettingsCopyKeys(\_:\_:) 

Function

# PMPrintSettingsCopyKeys(\_:\_:)

Obtains the keys for items in a print settings object.

macOS 10.5+

``` source
func PMPrintSettingsCopyKeys(
    _ printSettings: PMPrintSettings,
    _ settingsKeys: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`printSettings`  

The print settings object with the desired keys.

`settingsKeys`  

A pointer to your CFArray variable. On return, the variable refers to a Core Foundation array that contains the keys for items in the specified print settings object. Each of these keys may be passed to the function `PMPrintSettingsGetValue` to obtain a value. You are responsible for releasing the array. If an error occurs, the variable is set to `NULL`.

## Return Value

A result code. See Result Codes.

## Discussion

This function provides an array of the keys in a print settings object. You could get the values for the keys in the array with PMPrintSettingsGetValue(_:_:_:), or use the keys to look up the values in the dictionary returned by PMPrintSettingsCopyAsDictionary(_:_:).

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

func PMSetDuplex(PMPrintSettings, PMDuplexMode) -> OSStatus

Sets the duplex mode.

func PMPrintSettingsGetValue(PMPrintSettings, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFTypeRef>?>) -> OSStatus

Obtains the value of a setting in a print settings object.

func PMPrintSettingsSetValue(PMPrintSettings, CFString, CFTypeRef?, Bool) -> OSStatus

Stores the value of a setting in a print settings object.

func PMPrintSettingsCopyAsDictionary(PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

Creates a dictionary that contains the settings in a print settings object.

