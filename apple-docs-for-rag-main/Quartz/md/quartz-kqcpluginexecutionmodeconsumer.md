

- Quartz
-  kQCPlugInExecutionModeConsumer 

Global Variable

# kQCPlugInExecutionModeConsumer

A consumer execution mode. The custom patch always executes assuming the value of its Enable input port is `true`. (The Enable port is automatically added by the system.)

macOS 10.4+

``` source
var kQCPlugInExecutionModeConsumer: QCPlugInExecutionMode { get }
```

## See Also

### Constants

var kQCPlugInExecutionModeProvider: QCPlugInExecutionMode

A provider execution mode. The custom patch executes on demand—that is, whenever data is requested of it, but at most once per frame.

var kQCPlugInExecutionModeProcessor: QCPlugInExecutionMode

A processor execution mode. The custom patch executes whenever its inputs change or if the time change (assuming it’s time-dependent).

