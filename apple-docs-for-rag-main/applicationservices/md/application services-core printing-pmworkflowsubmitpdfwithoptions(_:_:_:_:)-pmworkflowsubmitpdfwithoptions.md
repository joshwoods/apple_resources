

- Application Services
- Core Printing
-  PMWorkflowSubmitPDFWithOptions(\_:\_:\_:\_:) 

Function

# PMWorkflowSubmitPDFWithOptions(\_:\_:\_:\_:)

Submits a PDF file for workflow processing using the specified CUPS options string.

macOS 10.3+

``` source
func PMWorkflowSubmitPDFWithOptions(
    _ workflowItem: CFURL,
    _ title: CFString?,
    _ options: UnsafePointer?,
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
| Executable tool | The tool is run with the following parameters: `title`, `options`, and `pdfFile`. |

`title`  

The user-displayable name of the PDF document.

`options`  

A string of CUPS-style key-value pairs that may be passed to the PDF workflow item. This parameter can be `NULL` in which case an empty string of options is used.

`pdfFile`  

A file system URL pointing to the PDF file to be processed by the workflow item.

## Return Value

A result code. See Result Codes.

## Discussion

The printing system uses this function in conjunction with the function PMWorkflowCopyItems(_:) to implement the PDF workflow button in the Print dialog.

## See Also

### Using PDF Workflow Items

func PMWorkflowCopyItems(UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains an array of the available PDF workflow items.

func PMWorkflowSubmitPDFWithSettings(CFURL, PMPrintSettings, CFURL) -> OSStatus

Submits a PDF file for workflow processing using the specified print settings.

