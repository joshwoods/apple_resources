

- Hypervisor
- Intel-based Mac
-  Hypervisor Errors 

API Collection

# Hypervisor Errors

Errors returned by Hypervisor functions.

## Topics

### Errors

var HV_SUCCESS: Int

The operation completed successfully.

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

var HV_DENIED: Int

The system didn’t allow the requested operation.

## See Also

### Common data types

typealias hv_return_t

The return type of framework functions.

