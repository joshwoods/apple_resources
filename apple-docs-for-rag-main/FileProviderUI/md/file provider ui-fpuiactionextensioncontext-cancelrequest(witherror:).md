

- File Provider UI
- FPUIActionExtensionContext
-  cancelRequest(withError:) 

Instance Method

# cancelRequest(withError:)

Cancels the action and returns the provided error.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.15+visionOS 1.0+

``` source
func cancelRequest(withError error: any Error)
```

## Mentioned in 

Adding Actions to the Context Menu

## Discussion

Call this method if the action fails. Set the error’s domain to FPUIErrorDomain. Set the error code to a FPUIExtensionErrorCode value.

## See Also

### Completing the Action

func completeRequest()

Marks the action as complete.

