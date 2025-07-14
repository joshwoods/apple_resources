

- Dispatch
- DispatchSource
- DispatchSource.ProcessEvent
-  exec 

Type Property

# exec

The process became another executable image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let exec: DispatchSource.ProcessEvent
```

## Discussion

The process has become another executable image via an `exec` or `posix_spawn` function family call.

## See Also

### Process Event Flags

static let all: DispatchSource.ProcessEvent

All process-related events.

static let exit: DispatchSource.ProcessEvent

The process has exited (perhaps cleanly, perhaps not).

static let fork: DispatchSource.ProcessEvent

The process created one or more child processes.

static let signal: DispatchSource.ProcessEvent

The process received a UNIX signal.

