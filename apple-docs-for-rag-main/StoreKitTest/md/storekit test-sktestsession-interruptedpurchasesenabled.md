

- StoreKit Test
- SKTestSession
-  interruptedPurchasesEnabled 

Instance Property

# interruptedPurchasesEnabled

A Boolean value that determines whether the test environment simulates an interrupted purchase.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var interruptedPurchasesEnabled: Bool { get set }
```

## Discussion

The default value is `false`. Enabling this property causes all purchases to fail until you disable it.

During testing, resolve the interrupted purchase by calling resolveIssueForTransaction(identifier:) for the affected transaction.

Changing this property overrides its setting in the StoreKit configuration file for this test session. Call resetToDefaultState() to revert all settings to those in the configuration file.

## See Also

### Testing interrupted purchases

func resolveIssueForTransaction(identifier: Int) throws

Simulates resolving an issue when you test interrupted purchases or billing retry scenarios.

