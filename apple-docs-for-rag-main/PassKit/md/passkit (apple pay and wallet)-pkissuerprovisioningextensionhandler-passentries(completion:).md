

- PassKit (Apple Pay and Wallet)
- PKIssuerProvisioningExtensionHandler
-  passEntries(completion:) 

Instance Method

# passEntries(completion:)

Reports the list of passes available to add to an iPhone.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func passEntries(completion: @escaping ([PKIssuerProvisioningExtensionPassEntry]) -> Void)
```

``` source
func passEntries() async -> [PKIssuerProvisioningExtensionPassEntry]
```

## Parameters 

`completion`  

A completion handler that the system calls to find the list of passes available to add to an iPhone. This handler takes the following parameter:

`entries`  
An array PKIssuerProvisioningExtensionPassEntry items that represents the passes that are available to add to Wallet.

## See Also

### Returning available passes

func remotePassEntries(completion: ([PKIssuerProvisioningExtensionPassEntry]) -> Void)

Reports the list of passes available to add to an Apple Watch.

class PKIssuerProvisioningExtensionPassEntry

An object that represents an item available to add to as a Wallet pass.

class PKIssuerProvisioningExtensionPaymentPassEntry

An object that represents a payment card available to add as a payment pass.

