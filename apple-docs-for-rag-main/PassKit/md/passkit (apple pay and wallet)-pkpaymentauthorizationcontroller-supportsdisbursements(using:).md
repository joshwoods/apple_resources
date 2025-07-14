

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationController
-  supportsDisbursements(using:) 

Type Method

# supportsDisbursements(using:)

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment network brands.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
class func supportsDisbursements(using supportedNetworks: [PKPaymentNetwork]) -> Bool
```

## Parameters 

`supportedNetworks`  

An array of `PKPaymentNetwork` elements to check.

## Return Value

true if the device supports processing disbursements through any of the specified networks; otherwise, false.

## See Also

### Determining whether the user can make payments or disbursements

class func canMakePayments() -> Bool

Returns whether the user can make payments.

class func canMakePayments(usingNetworks: [PKPaymentNetwork]) -> Bool

Returns whether the user can make payments through the specified network.

class func canMakePayments(usingNetworks: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns whether the user can make payments using a card from the specified network with the specified capabilities.

class func supportsDisbursements() -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests.

class func supportsDisbursements(using: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns a Boolean value indicating whether this device can process disbursement requests using the specified payment network brands and capabilities.

