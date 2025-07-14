

- Dispatch
- DispatchSource
- DispatchSource.ProcessEvent
-  all 

Type Property

# all

All process-related events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let all: DispatchSource.ProcessEvent
```

## See Also

### Process Event Flags

static let exec: DispatchSource.ProcessEvent

The process became another executable image.

static let exit: DispatchSource.ProcessEvent

The process has exited (perhaps cleanly, perhaps not).

static let fork: DispatchSource.ProcessEvent

The process created one or more child processes.

static let signal: DispatchSource.ProcessEvent

The process received a UNIX signal.

