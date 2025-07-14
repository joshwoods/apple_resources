

- Foundation
- RecoverableError
-  attemptRecovery(optionIndex:resultHandler:) 

Instance Method

# attemptRecovery(optionIndex:resultHandler:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func attemptRecovery(
    optionIndex recoveryOptionIndex: Int,
    resultHandler handler: @escaping (Bool) -> Void
)
```

**Required** Default implementation provided.

## Default Implementations

### RecoverableError Implementations

func attemptRecovery(optionIndex: Int, resultHandler: (Bool) -> Void)

