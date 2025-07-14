

- Application Services
- Core Printing
-  PMWorkflowSubmitPDFWithSettings(\_:\_:\_:) 

Function

# PMWorkflowSubmitPDFWithSettings(\_:\_:\_:)

Submits a PDF file for workflow processing using the specified print settings.

macOS 10.3+

``` source
func PMWorkflowSubmitPDFWithSettings(
    _ workflowItem: CFURL,
    _ settings: PMPrintSettings,
    _ pdfFile: CFURL
) -> OSStatus
```

## Parameters 

`workflowItem`  

A file system URL pointing to the workflow item that will handle the PDF file. See PMWorkflowCopyItems(_:). The following table describes the different types of workflow items for this function.

| Workflow item | Description |
|----|----|
| Automator action | The action is executed for the PDF file. Available in macOS 10.4 and later. |
| Folder alias | The PDF file is moved to the resolved folder. |
| Application or application alias | The application is sent an open event along with a reference to the PDF file. |
| Compiled AppleScript | The script is run with an open event along with a reference to the PDF file. |
| Executable tool | The tool is run with the specified settings and PDF file. This function converts these parameters into a CUPS options string and passes the options string to the tool. |

`settings`  

The print settings to apply to the PDF document. These settings are passed to the workflow item as a CUPS options string.

`pdfFile`  

A file system URL pointing to the PDF file to be processed by the workflow item.

## Return Value

A result code. See Result Codes.

## Discussion

The printing system uses this function in conjunction with the function PMWorkflowCopyItems(_:) to implement the PDF workflow button in the Print dialog.

### Special Considerations

In OS X v10.4 and earlier, this function is not implemented and returns an error. You can use the function PMWorkflowSubmitPDFWithOptions(_:_:_:_:) together with the function PMPrintSettingsToOptions(_:_:) instead.

## See Also

### Using PDF Workflow Items

func PMWorkflowCopyItems(UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains an array of the available PDF workflow items.

func PMWorkflowSubmitPDFWithOptions(CFURL, CFString?, UnsafePointer&lt;CChar>?, CFURL) -> OSStatus

Submits a PDF file for workflow processing using the specified CUPS options string.

