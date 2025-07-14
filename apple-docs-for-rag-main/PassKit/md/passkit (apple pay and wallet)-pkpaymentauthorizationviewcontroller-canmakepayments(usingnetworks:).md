

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewController
-  canMakePayments(usingNetworks:) 

Type Method

# canMakePayments(usingNetworks:)

Returns whether the user can make payments through the specified network.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
@MainActor
class func canMakePayments(usingNetworks supportedNetworks: [PKPaymentNetwork]) -> Bool
```

## Parameters 

`supportedNetworks`  

An array of payment networks, as listed in Payment Networks.

## Return Value

true if the user can make payments through any of the specified networks; otherwise, false.

## Discussion

User may not be able to make payments for a variety of reasons. For example, this functionality may not be supported by their hardware, or it may be restricted by parental controls.

If there are no configured payment cards, this method always returns false.

## See Also

### Determining whether the user can make payments

class func canMakePayments() -> Bool

Returns whether the user can make payments.

class func canMakePayments(usingNetworks: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns whether the user can make payments using a card from the specified network with the specified capabilities.

class func supportsDisbursements() -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests.

class func supportsDisbursements(using: [PKPaymentNetwork]) -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment networks.

class func supportsDisbursements(using: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment networks and merchant capabilities.

