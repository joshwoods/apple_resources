

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassViewControllerDelegate
-  addPaymentPassViewController(\_:didFinishAdding:error:) 

Instance Method

# addPaymentPassViewController(\_:didFinishAdding:error:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func addPaymentPassViewController(
    _ controller: PKAddPaymentPassViewController,
    didFinishAdding pass: PKPaymentPass?,
    error: (any Error)?
)
```

**Required**

## Parameters 

`controller`  

The controller adding the pass.

`pass`  

The completed pass, or `nil` if there was an error.

`error`  

If the request failed, this parameter contains an error object using the PKPassKitErrorDomain error domain. For a list of possible error codes, see the PKAddPaymentPassError enum.

## Discussion

This method is called when the request successfully adds the card to Apple Pay or when the request fails.

## See Also

### Requesting to add payment cards to Apple Pay

func addPaymentPassViewController(PKAddPaymentPassViewController, generateRequestWithCertificateChain: [Data], nonce: Data, nonceSignature: Data, completionHandler: (PKAddPaymentPassRequest) -> Void)

Asks the delegate to create an add payment request.

**Required**

class PKAddPaymentPassRequest

Contains the card data needed to add a card to Apple Pay.

