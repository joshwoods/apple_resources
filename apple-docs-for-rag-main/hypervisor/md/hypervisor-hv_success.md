

- Hypervisor
-  HV_SUCCESS 

Global Variable

# HV_SUCCESS

The operation completed successfully.

macOS

``` source
var HV_SUCCESS: Int { get }
```

## See Also

### Return Values

var HV_ERROR: Int

The operation was unsuccessful.

var HV_BUSY: Int

The operation was unsuccessful because the owning resource was busy.

var HV_BAD_ARGUMENT: Int

The operation was unsuccessful because the function call had an invalid argument.

var HV_NO_RESOURCES: Int

The operation was unsuccessful because the host had no resources available to complete the request.

var HV_NO_DEVICE: Int

The operation was unsuccessful because no VM or vCPU was available.

var HV_UNSUPPORTED: Int

The operation requested isn’t supported by the hypervisor.

