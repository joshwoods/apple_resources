

- Exposure Notification
- ENManager
-  preAuthorizeDiagnosisKeys(completionHandler:) 

Instance Method

# preAuthorizeDiagnosisKeys(completionHandler:)

Allows users to authorize a one-time release of diagnosis keys within five days of the authorization.

iOS 14.4+iPadOS 14.4+Mac Catalyst 14.4+

``` source
func preAuthorizeDiagnosisKeys(completionHandler: @escaping ENErrorHandler)
```

``` source
func preAuthorizeDiagnosisKeys() async throws
```

## Parameters 

`completionHandler`  

The completion handler the framework calls when the method completes.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func preAuthorizeDiagnosisKeys() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Important

Before requesting authorization, ensure the application is in the foreground.

This method prompts the user when getting tested to share their diagnosis keys if they receive a positive test result. An app should only call this method if it has a way to determine that the user is about to take a COVID test, such as apps that allow users to schedule testing appointments, and that can also determine if the result is positive.

The authorization duration is five days.

## See Also

### Preauthorizing Exposure Keys

func requestPreAuthorizedDiagnosisKeys(completionHandler: ENErrorHandler)

Requests diagnosis keys after the user authorizes sharing them.

typealias ENDiagnosisKeysAvailableHandler

The handler the system invokes after requesting diagnosis keys.

var diagnosisKeysAvailableHandler: ENDiagnosisKeysAvailableHandler?

The handler that receives available diagnosis keys after a successful preauthorization.

