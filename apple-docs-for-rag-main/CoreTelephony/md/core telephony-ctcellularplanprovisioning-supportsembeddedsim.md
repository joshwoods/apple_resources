

- Core Telephony
- CTCellularPlanProvisioning
-  supportsEmbeddedSIM 

Instance Property

# supportsEmbeddedSIM

A Boolean value that indicates whether the device has hardware eSIM support.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var supportsEmbeddedSIM: Bool { get }
```

## See Also

### Provisioning an eSIM

func supportsCellularPlan() -> Bool

Indicates whether the device supports eSIM and the activation policy allows eSIM installation.

func addPlan(with: CTCellularPlanProvisioningRequest, completionHandler: (CTCellularPlanProvisioningAddPlanResult) -> Void)

Starts the provisioning process for a specified eSIM.

enum CTCellularPlanProvisioningAddPlanResult

The result from attempting to provision an eSIM.

