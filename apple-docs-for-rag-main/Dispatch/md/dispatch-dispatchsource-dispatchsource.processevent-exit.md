

- Dispatch
- DispatchSource
- DispatchSource.ProcessEvent
-  exit 

Type Property

# exit

The process has exited (perhaps cleanly, perhaps not).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let exit: DispatchSource.ProcessEvent
```

## See Also

### Process Event Flags

static let all: DispatchSource.ProcessEvent

All process-related events.

static let exec: DispatchSource.ProcessEvent

The process became another executable image.

static let fork: DispatchSource.ProcessEvent

The process created one or more child processes.

static let signal: DispatchSource.ProcessEvent

The process received a UNIX signal.

