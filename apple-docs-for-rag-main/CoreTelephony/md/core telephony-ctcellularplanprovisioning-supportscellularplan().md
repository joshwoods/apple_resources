

- Core Telephony
- CTCellularPlanProvisioning
-  supportsCellularPlan() 

Instance Method

# supportsCellularPlan()

Indicates whether the device supports eSIM and the activation policy allows eSIM installation.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func supportsCellularPlan() -> Bool
```

## Return Value

true if the device supports eSIM and the activation policy allows eSIM installation; otherwise false.

## Discussion

This method checks that the device supports eSIM installation and verifies activation policies.

It doesn’t check whether the user has installed an eSIM. You can call this method at any time.

## See Also

### Provisioning an eSIM

var supportsEmbeddedSIM: Bool

A Boolean value that indicates whether the device has hardware eSIM support.

func addPlan(with: CTCellularPlanProvisioningRequest, completionHandler: (CTCellularPlanProvisioningAddPlanResult) -> Void)

Starts the provisioning process for a specified eSIM.

enum CTCellularPlanProvisioningAddPlanResult

The result from attempting to provision an eSIM.

