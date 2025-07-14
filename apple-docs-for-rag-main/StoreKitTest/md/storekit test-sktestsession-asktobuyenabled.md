

- StoreKit Test
- SKTestSession
-  askToBuyEnabled 

Instance Property

# askToBuyEnabled

A Boolean value that determines whether the testing environment simulates an Ask to Buy scenario.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var askToBuyEnabled: Bool { get set }
```

## Discussion

The default value is `false`. Enabling this property causes all purchases to require approval until you disable it. To approve the purchase in the testing environment, call approveAskToBuyTransaction(identifier:), and to decline it, call declineAskToBuyTransaction(identifier:).

Changing this property overrides its setting in the StoreKit configuration file for this test session. Call resetToDefaultState() to revert all settings to those in the configuration file.

## See Also

### Testing Ask To Buy transactions

func approveAskToBuyTransaction(identifier: Int) throws

Resolves an Ask to Buy test scenario by approving the transaction.

func declineAskToBuyTransaction(identifier: Int) throws

Resolves an Ask to Buy test scenario by declining the transaction.

