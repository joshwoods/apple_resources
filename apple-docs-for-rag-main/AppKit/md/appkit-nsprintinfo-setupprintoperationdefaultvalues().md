

- AppKit
- NSPrintInfo
-  setUpPrintOperationDefaultValues() 

Instance Method

# setUpPrintOperationDefaultValues()

Validates the attributes encapsulated by the print info.

macOS

``` source
func setUpPrintOperationDefaultValues()
```

## Discussion

Invoked when the print operation is about to start. Subclasses may override this method to set default values for any attributes that are not set.

## See Also

### Controlling Printing

var jobDisposition: NSPrintInfo.JobDisposition

The action specified for the job.

struct JobDisposition

Constants that specify values for the print job disposition.

