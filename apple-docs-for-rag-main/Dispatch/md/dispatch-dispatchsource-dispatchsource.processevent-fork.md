

- Dispatch
- DispatchSource
- DispatchSource.ProcessEvent
-  fork 

Type Property

# fork

The process created one or more child processes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let fork: DispatchSource.ProcessEvent
```

## See Also

### Process Event Flags

static let all: DispatchSource.ProcessEvent

All process-related events.

static let exec: DispatchSource.ProcessEvent

The process became another executable image.

static let exit: DispatchSource.ProcessEvent

The process has exited (perhaps cleanly, perhaps not).

static let signal: DispatchSource.ProcessEvent

The process received a UNIX signal.

