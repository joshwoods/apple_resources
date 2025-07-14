

- Quartz
- QCPlugIn
-  startExecution(\_:) Deprecated

Instance Method

# startExecution(\_:)

Allows you to perform custom setup tasks before the Quartz Composer engine starts rendering.

macOS 10.4–10.15Deprecated

``` source
func startExecution(_ context: (any QCPlugInContext)!) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`context`  

An opaque object , conforming to the QCPlugInContext protocol, that represents the execution context of the `QCPlugIn` object. Do not retain this object or use it outside of the scope of this method.

## Return Value

false indicates a fatal error occurred and prevents the Quartz Composer engine from starting.

## Discussion

The Quartz Composer engine calls this method when your custom patch starts to render. You can optionally override this execution method to perform setup tasks.

## See Also

### Performing Custom Tasks During Execution

func enableExecution((any QCPlugInContext)!)

Allows you to perform custom tasks when the execution of the `QCPlugIn` object is resumed.

Deprecated

func disableExecution((any QCPlugInContext)!)

Allows you to perform custom tasks when the execution of the `QCPlugIn` object is paused.

Deprecated

func stopExecution((any QCPlugInContext)!)

Allows you to perform custom tasks when the `QCPlugIn` object stops executing.

Deprecated

