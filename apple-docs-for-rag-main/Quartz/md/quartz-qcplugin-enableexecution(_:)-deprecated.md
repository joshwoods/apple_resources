

- Quartz
- QCPlugIn
-  enableExecution(\_:) Deprecated

Instance Method

# enableExecution(\_:)

Allows you to perform custom tasks when the execution of the `QCPlugIn` object is resumed.

macOS 10.4–10.15Deprecated

``` source
func enableExecution(_ context: (any QCPlugInContext)!)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`context`  

An opaque object , conforming to the QCPlugInContext protocol, that represents the execution context of the `QCPlugIn` object. Do not retain this object or use it outside of the scope of this method.

## Discussion

The Quartz Composer engine calls this method when results start to be pulled from the custom patch. You can optionally override this execution method to perform custom tasks at that time.

## See Also

### Performing Custom Tasks During Execution

func startExecution((any QCPlugInContext)!) -> Bool

Allows you to perform custom setup tasks before the Quartz Composer engine starts rendering.

Deprecated

func disableExecution((any QCPlugInContext)!)

Allows you to perform custom tasks when the execution of the `QCPlugIn` object is paused.

Deprecated

func stopExecution((any QCPlugInContext)!)

Allows you to perform custom tasks when the `QCPlugIn` object stops executing.

Deprecated

