

- Hypervisor
-  HV_EXIT_REASON_VTIMER_ACTIVATED 

Global Variable

# HV_EXIT_REASON_VTIMER_ACTIVATED

The value that identifies when the virtual timer enters the pending state.

macOS

``` source
var HV_EXIT_REASON_VTIMER_ACTIVATED: hv_exit_reason_t { get }
```

## See Also

### Exit Reasons

var HV_EXIT_REASON_CANCELED: hv_exit_reason_t

The value that identifies exits requested by exit handler on the host.

var HV_EXIT_REASON_EXCEPTION: hv_exit_reason_t

The value that identifies traps caused by the guest operations.

var HV_EXIT_REASON_UNKNOWN: hv_exit_reason_t

The value that identifies unexpected exits.

