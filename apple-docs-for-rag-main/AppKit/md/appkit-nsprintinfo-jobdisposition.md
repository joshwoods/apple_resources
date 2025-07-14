

- AppKit
- NSPrintInfo
-  jobDisposition 

Instance Property

# jobDisposition

The action specified for the job.

macOS

``` source
var jobDisposition: NSPrintInfo.JobDisposition { get set }
```

## Discussion

One of the following value:

- spool is a normal print job.

- preview sends the print job to the Preview application.

- save saves the print job to a file.

- cancel aborts the print job.

## See Also

### Controlling Printing

struct JobDisposition

Constants that specify values for the print job disposition.

func setUpPrintOperationDefaultValues()

Validates the attributes encapsulated by the print info.

