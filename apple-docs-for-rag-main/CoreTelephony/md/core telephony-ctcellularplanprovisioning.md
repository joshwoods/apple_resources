

- Core Telephony
-  CTCellularPlanProvisioning 

Class

# CTCellularPlanProvisioning

An object you use to download and install a carrier eSIM.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CTCellularPlanProvisioning
```

## Overview

This class is only available to carrier apps with suitable entitlements.

## Topics

### Provisioning an eSIM

func supportsCellularPlan() -> Bool

Indicates whether the device supports eSIM and the activation policy allows eSIM installation.

var supportsEmbeddedSIM: Bool

A Boolean value that indicates whether the device has hardware eSIM support.

func addPlan(with: CTCellularPlanProvisioningRequest, completionHandler: (CTCellularPlanProvisioningAddPlanResult) -> Void)

Starts the provisioning process for a specified eSIM.

enum CTCellularPlanProvisioningAddPlanResult

The result from attempting to provision an eSIM.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### eSIM

class CTCellularPlanProvisioningRequest

A request specifying an eSIM to download and install.

