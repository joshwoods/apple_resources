

- PassKit (Apple Pay and Wallet)
- PKIssuerProvisioningExtensionHandler
-  status(completion:) 

Instance Method

# status(completion:)

Reports the status of your Wallet extension.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func status(completion: @escaping (PKIssuerProvisioningExtensionStatus) -> Void)
```

``` source
func status() async -> PKIssuerProvisioningExtensionStatus
```

## Parameters 

`completion`  

A completion handler that the system calls to determine if there is a pass available and if adding the pass requires authentication. This handler takes the following parameter:

`status`  
A PKIssuerProvisioningExtensionStatus that indicates whether there are any payment cards available to add as Wallet passes.

## See Also

### Returning extension status

class PKIssuerProvisioningExtensionStatus

An object that indicates whether there are any payment cards available to add as Wallet passes.

