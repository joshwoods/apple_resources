

- ManagedAppDistribution
- ManagedAppDistributionError
-  attemptRecovery(optionIndex:resultHandler:) 

Instance Method

# attemptRecovery(optionIndex:resultHandler:)

Attempt to recover from this error when someone selects the option at the given index.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
func attemptRecovery(
    optionIndex recoveryOptionIndex: Int,
    resultHandler handler: @escaping (Bool) -> Void
)
```

## See Also

### Recovering from errors

func attemptRecovery(optionIndex: Int) -> Bool

Attempt to recover from this error when someone selects the option at the given index.

