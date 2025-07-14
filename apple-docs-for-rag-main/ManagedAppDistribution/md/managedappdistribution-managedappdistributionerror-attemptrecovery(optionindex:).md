

- ManagedAppDistribution
- ManagedAppDistributionError
-  attemptRecovery(optionIndex:) 

Instance Method

# attemptRecovery(optionIndex:)

Attempt to recover from this error when someone selects the option at the given index.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
func attemptRecovery(optionIndex recoveryOptionIndex: Int) -> Bool
```

## Return Value

`true` to indicate successful recovery; otherwise `false`.

## See Also

### Recovering from errors

func attemptRecovery(optionIndex: Int, resultHandler: (Bool) -> Void)

Attempt to recover from this error when someone selects the option at the given index.

