

- Application Services
- Core Printing
-  PMGetCollate(\_:\_:) 

Function

# PMGetCollate(\_:\_:)

Obtains a Boolean value that indicates whether the job collate option is selected.

macOS 10.2+

``` source
func PMGetCollate(
    _ printSettings: PMPrintSettings,
    _ collate: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`printSettings`  

The print settings object you’re querying to determine whether the job collate option is selected.

`collate`  

A pointer to your Boolean variable. On return, `true` if the job collate option is selected; otherwise, `false`.

## Return Value

A result code. See Result Codes.

## Discussion

The Collated checkbox is displayed in the Copies & Pages pane of the Print dialog. This option determines how printed material is organized. For example, if you have a document that is three pages long and you are printing multiple copies with the Collated option selected, the job prints pages 1, 2, and 3 in that order and then repeats. However, if the Collated option is not selected and you’re printing multiple copies of those same three pages, the job prints copies of page 1, then copies of page 2, and finally copies of page 3.

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

func PMPrintSettingsCopyKeys(PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains the keys for items in a print settings object.

