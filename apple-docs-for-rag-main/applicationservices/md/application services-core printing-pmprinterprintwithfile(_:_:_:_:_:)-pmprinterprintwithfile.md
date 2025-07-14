

- Application Services
- Core Printing
-  PMPrinterPrintWithFile(\_:\_:\_:\_:\_:) 

Function

# PMPrinterPrintWithFile(\_:\_:\_:\_:\_:)

Submits a print job to a specified printer using a file that contains print data.

macOS 10.3+

``` source
func PMPrinterPrintWithFile(
    _ printer: PMPrinter,
    _ settings: PMPrintSettings,
    _ format: PMPageFormat?,
    _ mimeType: CFString?,
    _ fileURL: CFURL
) -> OSStatus
```

## Parameters 

`printer`  

The destination printer.

`settings`  

The print settings for the print job.

`format`  

The physical page size and orientation with which the document should be printed. This parameter can be `NULL`.

`mimeType`  

The MIME type of the data to be printed. If this parameter is `NULL`, the MIME type will be determined automatically. You can obtain a list of the MIME types supported by a given printer using the function PMPrinterGetMimeTypes(_:_:_:).

`fileURL`  

The URL of the file that supplies the print data.

## Return Value

A result code. See Result Codes. If the specified printer cannot handle the file's MIME type, a non-zero error code is returned.

## Discussion

This function can fail if the specified printer cannot handle the file’s MIME type. Use the function PMPrinterGetMimeTypes(_:_:_:) to check whether a MIME type is supported.

## See Also

### Submitting a Print Job to a Printer

func PMPrinterPrintWithProvider(PMPrinter, PMPrintSettings, PMPageFormat?, CFString, CGDataProvider) -> OSStatus

Submits a print job to a specified printer using a Quartz data provider to obtain the print data.

