

- ProximityReader
- PaymentCardReader
-  relinkAccount(using:) 

Instance Method

# relinkAccount(using:)

Presents a sheet for the merchant to re-accept Tap to Pay on iPhone’s Terms and Conditions on a device using a different Apple Account.

iOS 16.1+iPadOS 16.1+Mac Catalyst 17.0+

``` source
func relinkAccount(using token: PaymentCardReader.Token) async throws
```

## Parameters 

`token`  

The token from your payment service provider. This token contains the merchant identifier and must include permission for relinking.

## Discussion

To use Tap to Pay on iPhone, your participating payment service provider must provide the merchant using your app with a secure token. This token contains a unique identifier for each merchant and also specifies if relinking using a different Apple Account is allowed.

To use this method, a merchant must have already accepted the Terms and Conditions using linkAccount(using:).

After a merchant accepts the Terms and Conditions for their specific merchant identifier on one device, they don’t need to accept it again on additional devices that use the same identifier.

Throws

PaymentCardReaderError.accountLinkingFailed, PaymentCardReaderError.accountLinkingCancelled, or other relevant errors in PaymentCardReaderError.

## See Also

### Displaying the Tap to Pay on iPhone’s terms and conditions

func isAccountLinked(using: PaymentCardReader.Token) async throws -> Bool

A Boolean value that indicates whether the account is already linked.

func linkAccount(using: PaymentCardReader.Token) async throws

Presents a sheet for the merchant to accept Tap to Pay on iPhone’s Terms and Conditions on a device.

struct Token

A secure token that you receive from your participating payment service provider.

