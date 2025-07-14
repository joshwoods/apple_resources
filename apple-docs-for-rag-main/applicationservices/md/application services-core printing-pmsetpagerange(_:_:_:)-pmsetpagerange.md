

- Application Services
- Core Printing
-  PMSetPageRange(\_:\_:\_:) 

Function

# PMSetPageRange(\_:\_:\_:)

Sets the valid range of pages that can be printed.

macOS 10.0+

``` source
func PMSetPageRange(
    _ printSettings: PMPrintSettings,
    _ minPage: UInt32,
    _ maxPage: UInt32
) -> OSStatus
```

## Parameters 

`printSettings`  

The print settings object whose page range you want to set.

`minPage`  

The minimum page number allowed. This value appears as the default in the From field of the Print dialog.

`maxPage`  

The maximum page number allowed. This value appears as the default in the To field of the Print dialog. Pass the constant `kPMPrintAllPages` to allow the user to print the entire document. If the first page is set to 1, then passing `kPMPrintAllPages` as the maximum page number causes the All button to be selected.

## Return Value

A result code. See Result Codes.

## Discussion

The function `PMSetPageRange` allows applications to set the minimum and maximum page numbers that can be printed for a document. If the user enters a value outside of this range in the Print dialog, the value is set to the closest allowed value. You can use the PMGetFirstPage(_:_:) and PMGetLastPage(_:_:) functions to obtain the values entered by the user in the Print dialog.)

If you call the function `PMSetPageRange` to set the maximum page to a value other than the constant `kPMPrintAllPages`, the function `PMSetPageRange` causes the page range in the Print dialog to be properly restricted to the specified range. If you call the function `PMSetPageRange` without also calling the functions `PMSetFirstPage` or `PMSetLastPage`, then the Print dialog shows the specified page range in the From and To fields but with the All button selected. If you call the function `PMSetPageRange` and then call `PMSetFirstPage` or `PMSetLastPage` using the same page range you specified for `PMSetPageRange`, then the Print dialog shows the From button selected.

In all cases, if your application sets a range with `PMSetPageRange` and subsequently calls PMSetFirstPage(_:_:_:) or PMSetLastPage(_:_:_:) with values outside of the specified range, Core Printing returns a result code of `kPMValueOutOfRange`. Conversely, if your application calls `PMSetPageRange` after calling `PMSetFirstPage` or `PMSetLastPage` (or after displaying the Print dialog), the page range specified by `PMSetPageRange` takes precedence, and the first and last page values are adjusted accordingly.

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

func PMPrintSettingsCopyKeys(PMPrintSettings, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains the keys for items in a print settings object.

