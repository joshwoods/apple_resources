

- StoreKit Test
- SKTestSession
-  declinePriceIncreaseForTransaction(identifier:) 

Instance Method

# declinePriceIncreaseForTransaction(identifier:)

Simulates a user canceling an auto-renewable subscription by disabling auto-renew.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
func declinePriceIncreaseForTransaction(identifier: Int) throws
```

## Parameters 

`identifier`  

The transaction identifier of the auto-renewable subscription that has a pending price increase.

## Discussion

To test how your app handles the price increase consent flow for auto-renewable subscriptions, first call requestPriceIncreaseConsentForTransaction(identifier:).

Call declinePriceIncreaseForTransaction(identifier:) to simulate a user canceling the subscription. Specifically, this method disables auto-renew and removes the subscription’s pending price increase status. The subscription expires at the end of the billing period in the testing environment.

## See Also

### Testing price increase consent

func requestPriceIncreaseConsentForTransaction(identifier: Int) throws

Simulates a price increase that requires customer consent for an auto-renewable subscription.

func consentToPriceIncreaseForTransaction(identifier: Int) throws

Simulates a user consenting to a price increase for an auto-renewable subscription.

