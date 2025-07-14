

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewController
-  supportsDisbursements() 

Type Method

# supportsDisbursements()

Returns a Boolean value that indicates whether this device can process disbursement requests.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor
class func supportsDisbursements() -> Bool
```

## Return Value

true if the device can process disbursement requests; otherwise, false.

## See Also

### Determining whether the user can make payments

class func canMakePayments() -> Bool

Returns whether the user can make payments.

class func canMakePayments(usingNetworks: [PKPaymentNetwork]) -> Bool

Returns whether the user can make payments through the specified network.

class func canMakePayments(usingNetworks: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns whether the user can make payments using a card from the specified network with the specified capabilities.

class func supportsDisbursements(using: [PKPaymentNetwork]) -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment networks.

class func supportsDisbursements(using: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment networks and merchant capabilities.

