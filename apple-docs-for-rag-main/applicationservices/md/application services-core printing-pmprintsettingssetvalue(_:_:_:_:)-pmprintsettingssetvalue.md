

- Application Services
- Core Printing
-  PMPrintSettingsSetValue(\_:\_:\_:\_:) 

Function

# PMPrintSettingsSetValue(\_:\_:\_:\_:)

Stores the value of a setting in a print settings object.

macOS 10.4+

``` source
func PMPrintSettingsSetValue(
    _ printSettings: PMPrintSettings,
    _ key: CFString,
    _ value: CFTypeRef?,
    _ locked: Bool
) -> OSStatus
```

## Parameters 

`printSettings`  

The print settings object you want to update.

`key`  

A string constant that specifies the key for the desired setting. Some keys are currently defined in `PMTicket.h`; other keys are user-defined.

`value`  

A Core Foundation object that corresponds to the specified key. If you pass `NULL`, any existing setting for the specified key is removed.

`locked`  

If `true`, the item being set should be locked; otherwise, `false`. Currently, you should always pass `false`.

## Return Value

A result code. See Result Codes.

## Discussion

This function makes it possible to add, change, or remove print settings directly. Print settings are stored as key-value pairs. The keys are Core Foundation strings and the corresponding values are Core Foundation objects.

You can use this function to store user-defined data in a print settings object. You should make sure that the custom keys you define for your private data do not conflict with any other keys in the object. Each data item you store needs to be a Core Foundation object. You can use the function `PMPrintSettingsGetValue` to retrieve your private data.

If you call this function after initiating a print job (for example, by calling `PMSessionBeginCGDocument`), the change is ignored for the current job.

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

func PMPrintSettingsCopyAsDictionary(PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

Creates a dictionary that contains the settings in a print settings object.

func PMPrintSettingsCopyKeys(PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains the keys for items in a print settings object.

