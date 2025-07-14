

- PassKit (Apple Pay and Wallet)
- PKIssuerProvisioningExtensionHandler
-  remotePassEntries(completion:) 

Instance Method

# remotePassEntries(completion:)

Reports the list of passes available to add to an Apple Watch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func remotePassEntries(completion: @escaping ([PKIssuerProvisioningExtensionPassEntry]) -> Void)
```

``` source
func remotePassEntries() async -> [PKIssuerProvisioningExtensionPassEntry]
```

## Parameters 

`completion`  

A completion handler that the system calls to find the list of passes available to add to an Apple Watch. This handler takes the following parameter:

`entries`  
An array PKIssuerProvisioningExtensionPassEntry items representing the passes that are available to add to Wallet.

## See Also

### Returning available passes

func passEntries(completion: ([PKIssuerProvisioningExtensionPassEntry]) -> Void)

Reports the list of passes available to add to an iPhone.

class PKIssuerProvisioningExtensionPassEntry

An object that represents an item available to add to as a Wallet pass.

class PKIssuerProvisioningExtensionPaymentPassEntry

An object that represents a payment card available to add as a payment pass.

