

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewController
-  supportsDisbursements(using:capabilities:) 

Type Method

# supportsDisbursements(using:capabilities:)

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment networks and merchant capabilities.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor
class func supportsDisbursements(
    using supportedNetworks: [PKPaymentNetwork],
    capabilities: PKMerchantCapability
) -> Bool
```

## Parameters 

`supportedNetworks`  

An array of payment networks to check.

`capabilities`  

One of the PKMerchantCapability `capabilities.`

## Return Value

true if the device can process disbursement requests using the specified payment networks and merchant capabilities; otherwise, false.

## See Also

### Determining whether the user can make payments

class func canMakePayments() -> Bool

Returns whether the user can make payments.

class func canMakePayments(usingNetworks: [PKPaymentNetwork]) -> Bool

Returns whether the user can make payments through the specified network.

class func canMakePayments(usingNetworks: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns whether the user can make payments using a card from the specified network with the specified capabilities.

class func supportsDisbursements() -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests.

class func supportsDisbursements(using: [PKPaymentNetwork]) -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment networks.

