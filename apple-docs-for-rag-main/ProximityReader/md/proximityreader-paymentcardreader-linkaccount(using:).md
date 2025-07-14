

- ProximityReader
- PaymentCardReader
-  linkAccount(using:) 

Instance Method

# linkAccount(using:)

Presents a sheet for the merchant to accept Tap to Pay on iPhone’s Terms and Conditions on a device.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
func linkAccount(using token: PaymentCardReader.Token) async throws
```

## Parameters 

`token`  

The token from your payment service provider. This token contains the merchant identifier.

## Mentioned in 

Adding support for Tap to Pay on iPhone to your app

## Discussion

To use Tap to Pay on iPhone, your participating payment service provider must provide the merchant using your app with a secure token. This token contains an unique identifier for each merchant. This merchant must accept Tap to Pay on iPhone’s Terms and Conditions. After a merchant accepts the Terms and Conditions for their specific merchant identifier on one device, they don’t need to accept it again on additional devices that use the same identifier.

Use the isAccountLinked(using:) method to confirm calling linkAccount(using:) is required.

If the merchant hasn’t accepted the Terms and Conditions, calling prepare(using:) throws PaymentCardReaderError.accountNotLinked.

If the merchant has already accepted the Terms and Conditions, calling this method throws PaymentCardReaderError.accountAlreadyLinked.

Throws

PaymentCardReaderError.accountAlreadyLinked if the merchant already accepted the Tap to Pay on iPhone’s Terms and Conditions. The method throws PaymentCardReaderError.accountLinkingFailed, PaymentCardReaderError.accountLinkingCancelled, or other relevant errors in PaymentCardReaderError if a problem occurs.

## See Also

### Displaying the Tap to Pay on iPhone’s terms and conditions

func isAccountLinked(using: PaymentCardReader.Token) async throws -> Bool

A Boolean value that indicates whether the account is already linked.

func relinkAccount(using: PaymentCardReader.Token) async throws

Presents a sheet for the merchant to re-accept Tap to Pay on iPhone’s Terms and Conditions on a device using a different Apple Account.

struct Token

A secure token that you receive from your participating payment service provider.

