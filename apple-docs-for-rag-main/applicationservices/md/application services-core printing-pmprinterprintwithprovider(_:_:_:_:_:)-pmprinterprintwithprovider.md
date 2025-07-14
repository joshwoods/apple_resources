

- Application Services
- Core Printing
-  PMPrinterPrintWithProvider(\_:\_:\_:\_:\_:) 

Function

# PMPrinterPrintWithProvider(\_:\_:\_:\_:\_:)

Submits a print job to a specified printer using a Quartz data provider to obtain the print data.

macOS 10.3+

``` source
func PMPrinterPrintWithProvider(
    _ printer: PMPrinter,
    _ settings: PMPrintSettings,
    _ format: PMPageFormat?,
    _ mimeType: CFString,
    _ provider: CGDataProvider
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

The MIME type of the data to be printed. This parameter cannot be `NULL`. If you want automatic typing, use the function PMPrinterPrintWithFile(_:_:_:_:_:) instead. You can obtain a list of the MIME types supported by a given printer using the function PMPrinterGetMimeTypes(_:_:_:).

`provider`  

The data provider that supplies the print data.

## Return Value

A result code. See Result Codes.

## Discussion

This function can fail if the specified printer cannot handle the data provider’s MIME type. Use the function PMPrinterGetMimeTypes(_:_:_:) to check whether a MIME type is supported.

### Special Considerations

In OS X v10.4 and earlier, this function is not implemented and returns the error code –1 when called. You can write your print data to a file and use `PMPrinterPrintWithFile` instead.

## See Also

### Submitting a Print Job to a Printer

func PMPrinterPrintWithFile(PMPrinter, PMPrintSettings, PMPageFormat?, CFString?, CFURL) -> OSStatus

Submits a print job to a specified printer using a file that contains print data.

