

- Core Telephony
- CTCellularPlanProvisioning
-  addPlan(with:completionHandler:) 

Instance Method

# addPlan(with:completionHandler:)

Starts the provisioning process for a specified eSIM.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func addPlan(
    with request: CTCellularPlanProvisioningRequest,
    completionHandler: @escaping (CTCellularPlanProvisioningAddPlanResult) -> Void
)
```

``` source
func addPlan(with request: CTCellularPlanProvisioningRequest) async -> CTCellularPlanProvisioningAddPlanResult
```

## Parameters 

`request`  

A CTCellularPlanProvisioningRequest that identifies the eSIM to download.

`completionHandler`  

A completion handler that executes after processing the request. The parameter passed to the completion handler indicates whether the request succeeded, failed, or ended in an unknown state.

## Discussion

Once your app calls this method, an iOS wizard guides the user through the process of installing and configuration an eSIM.

### Installing an eSIM in the Background

The user may send your app to the background prior to completing eSIM installation. To ensure your app has an opportunity to execute the completion handler and get the result of the installation, use beginBackgroundTask(expirationHandler:) to perform the eSIM installation as a background task.

## See Also

### Provisioning an eSIM

func supportsCellularPlan() -> Bool

Indicates whether the device supports eSIM and the activation policy allows eSIM installation.

var supportsEmbeddedSIM: Bool

A Boolean value that indicates whether the device has hardware eSIM support.

enum CTCellularPlanProvisioningAddPlanResult

The result from attempting to provision an eSIM.

