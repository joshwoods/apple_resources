

- StoreKit Test
- SKTestSession
-  clearTransactions() 

Instance Method

# clearTransactions()

Removes all transactions from the test environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func clearTransactions()
```

## Discussion

After you clear the transactions from the test environment, the test environment produces an empty receipt. Use this method to enable repeating tests for one-time purchases.

To revert all the settings in the test environment to those in the StoreKit configuration file, see resetToDefaultState().

## See Also

### Managing transactions in the test environment

func allTransactions() -> [SKTestTransaction]

Gets a list of all transactions in the test environment.

func deleteTransaction(identifier: Int) throws

Deletes a specific transaction from the test environment.

