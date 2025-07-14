

- File Provider
- NSFileProviderManager
-  signalErrorResolved(\_:completionHandler:) 

Instance Method

# signalErrorResolved(\_:completionHandler:)

Indicates a resolved error.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func signalErrorResolved(
    _ error: any Error,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func signalErrorResolved(_ error: any Error) async throws
```

## Parameters 

`error`  

The original error.

`completionHandler`  

A block that the system calls after resuming the action that triggered the original error. The block takes the following parameters:

error  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func signalErrorResolved(_ error: any Error) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method if any of your extension’s actions fail because of an NSFileProviderError.Code.notAuthenticated, NSFileProviderError.Code.insufficientQuota, or NSFileProviderError.Code.serverUnreachable error. As soon as you resolve the underlying error, call this method to tell the system to retry the original action.

