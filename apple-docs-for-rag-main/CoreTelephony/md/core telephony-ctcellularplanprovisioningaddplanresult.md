

- Core Telephony
-  CTCellularPlanProvisioningAddPlanResult 

Enumeration

# CTCellularPlanProvisioningAddPlanResult

The result from attempting to provision an eSIM.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.10+

``` source
enum CTCellularPlanProvisioningAddPlanResult
```

## Topics

### Results

case fail

The requested eSIM provisioning failed.

case success

The requested eSIM provisioning succeeded.

case unknown

The result of the requested eSIM provisioning is unknown.

case cancel

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Provisioning an eSIM

func supportsCellularPlan() -> Bool

Indicates whether the device supports eSIM and the activation policy allows eSIM installation.

var supportsEmbeddedSIM: Bool

A Boolean value that indicates whether the device has hardware eSIM support.

func addPlan(with: CTCellularPlanProvisioningRequest, completionHandler: (CTCellularPlanProvisioningAddPlanResult) -> Void)

Starts the provisioning process for a specified eSIM.

