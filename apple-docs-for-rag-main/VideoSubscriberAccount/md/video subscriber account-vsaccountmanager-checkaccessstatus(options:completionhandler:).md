

- Video Subscriber Account
- VSAccountManager
-  checkAccessStatus(options:completionHandler:) 

Instance Method

# checkAccessStatus(options:completionHandler:)

Checks your app’s access to user subscription information, and requests access if needed.

iOS 10.0+iPadOS 10.0+tvOS 10.0+visionOS 1.0+

``` source
func checkAccessStatus(
    options: [VSCheckAccessOption : Any] = [:],
    completionHandler: @escaping (VSAccountAccessStatus, (any Error)?) -> Void
)
```

``` source
func checkAccessStatus(options: [VSCheckAccessOption : Any] = [:]) async throws -> VSAccountAccessStatus
```

## Parameters 

`options`  

The options you use to check access status. See VSCheckAccessOption for a list of possible options.

`completionHandler`  

The closure the account manager executes after it checks your app’s access status. This closure has no return value and takes the following parameters:

accessStatus  
The access status of your app. For a list of possible values, see VSAccountAccessStatus.

error  
An error object that contains information about a problem, or `nil` if the operation completed successfully.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Checking Access Status

struct VSCheckAccessOption

The options your app uses when checking access status.

enum VSAccountAccessStatus

Constants that represent your app’s access status to the user’s subscription information.

