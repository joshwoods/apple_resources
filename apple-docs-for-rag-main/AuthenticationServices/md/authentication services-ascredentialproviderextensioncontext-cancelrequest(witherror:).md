

- Authentication Services
- ASCredentialProviderExtensionContext
-  cancelRequest(withError:) 

Instance Method

# cancelRequest(withError:)

Cancels the request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func cancelRequest(withError error: any Error)
```

## Parameters 

`error`  

Use an error domain of ASExtensionErrorDomain and a code of type ASExtensionError.Code.

## Mentioned in 

Providing one-time passcodes to AutoFill

## Discussion

Call this method if the user cancels the action or if a failure occurs. The system dismisses your extension’s view controller automatically.

