

- ProximityReader
- PaymentCardReader
-  isAccountLinked(using:) 

Instance Method

# isAccountLinked(using:)

A Boolean value that indicates whether the account is already linked.

iOS 16.4+iPadOS 16.4+Mac Catalyst 17.0+

``` source
func isAccountLinked(using token: PaymentCardReader.Token) async throws -> Bool
```

## Parameters 

`token`  

The token from your payment service provider. This token contains the merchant identifier.

## Discussion

Call linkAccount(using:) to link an account.

Note

If prepare(using:) throws an PaymentCardReaderError.accountNotLinked error call linkAccount(using:) again to relink the account.

Throws

PaymentCardReaderError

## See Also

### Displaying the Tap to Pay on iPhone’s terms and conditions

func linkAccount(using: PaymentCardReader.Token) async throws

Presents a sheet for the merchant to accept Tap to Pay on iPhone’s Terms and Conditions on a device.

func relinkAccount(using: PaymentCardReader.Token) async throws

Presents a sheet for the merchant to re-accept Tap to Pay on iPhone’s Terms and Conditions on a device using a different Apple Account.

struct Token

A secure token that you receive from your participating payment service provider.

