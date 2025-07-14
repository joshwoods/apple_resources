

- Application Services
- Core Printing
-  PMWorkflowCopyItems(\_:) 

Function

# PMWorkflowCopyItems(\_:)

Obtains an array of the available PDF workflow items.

macOS 10.3+

``` source
func PMWorkflowCopyItems(_ workflowItems: UnsafeMutablePointer?>) -> OSStatus
```

## Parameters 

`workflowItems`  

A pointer to your CFArray variable. On return, the variable refers to an Core Foundation array. Each element in the array is a dictionary that describes either a PDF workflow item or a folder containing a set of PDF workflow items. For a list of possible keys, see PDF Workflow Dictionary Keys. You are responsible for releasing the array.

## Return Value

A result code. See Result Codes.

## See Also

### Using PDF Workflow Items

func PMWorkflowSubmitPDFWithOptions(CFURL, CFString?, UnsafePointer&lt;CChar>?, CFURL) -> OSStatus

Submits a PDF file for workflow processing using the specified CUPS options string.

func PMWorkflowSubmitPDFWithSettings(CFURL, PMPrintSettings, CFURL) -> OSStatus

Submits a PDF file for workflow processing using the specified print settings.

