

- StoreKit Test
- SKTestSession
-  resetToDefaultState() 

Instance Method

# resetToDefaultState()

Removes all property overrides and resets all test session settings to their default state.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func resetToDefaultState()
```

## Discussion

During testing, your tests may override the property settings such as the timeRate, askToBuyEnabled, interruptedPurchasesEnabled, and billingGracePeriodIsEnabled. Call this method to revert all the property settings to the states defined in the StoreKit configuration file that you use to initialize this SKTestSession instance.

See clearTransactions() to remove all transactions from the testing environment.

## See Also

### Initializing test sessions

convenience init(configurationFileNamed: String) throws

Initializes the test session with the provided configuration file that you include in your application’s bundle.

init(contentsOf: URL) throws

Initializes the test session with a configuration file you provide through a URL.

